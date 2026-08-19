# A sense index—what records mean, not what they say, and which to open first

**Oleksii Zagorskyi** · August 19, 2026

*This is a pattern for making a body of text records answerable by meaning: the shape of an index and the reasoning that gives it that shape, built differently for every corpus that adopts it. Give it to the agent that works your records; the choices it will ask you to make are named below.*

A sense index makes a body of text records too large for one reading context cheaply answerable. It answers *which records carry this idea, and which few should I read first?* without your agent re-reading the body each time you ask. Its entries are senses, not words: a record is listed under an idea it carries even when the idea's keywords never appear in the text. The records under every entry are ranked, so the index says not only where a sense lives but where it lives centrally. It pays off on repeated asking, when new records keep arriving or you keep returning with new questions—and never on a single read. At large scale you would reach for a vector database and a retrieval pipeline—below it they are overkill, which is exactly the gap this index fills. The pattern described here is in my daily use on a working business corpus of text—hundreds of records under more than ten lenses. But the examples are synthetic: a CRM filling with customer records, and a corpus of ancient Greek myths, one file per myth, queried by a teacher who keeps returning with new questions.

## When the same records must answer, session after session

The situation is a folder of text records that keeps being asked—meeting notes, CRM histories, support tickets, a teaching canon—with an agent doing the reading: fresh records against standing questions, or fresh questions against a standing corpus, unit by unit.

And the reading does not accumulate. The session asking today is often not the one that read yesterday—so whatever one pass learned is gone by the next. A single session that could read everything would need no index: it already holds everything. The index exists because readings die with their sessions—and because reading the whole corpus is expensive.

## Finding a meaning might cost a full re-read, and not every mention of it weighs the same

The re-read half first. Word search returns the records that use a word and misses the ones that mean it—the idea was never phrased with your keyword, and incidental uses flood the results. Semantic search fixes the words and keeps the reading: a model retrieves by meaning well enough, but what comes back is a neighborhood of similar passages, rebuilt at every query and kept nowhere. To know which records matter, your agent still reads through what the search returned; and the next session, with the next question, pays the same reading again.

Then the gravity half. Mentions are not equal: one record is built around an idea, ten records touch it in passing, and every instrument above returns them flat. Similarity scores are not centrality. A summary written over the whole pile is no flatter cure—the newest, loudest material writes it, and a record that mentions a theme once weighs the same as the record the theme lives in.

If a single strongly worded recent record can skew your sense of the whole, this is the shape the pattern below is built against.

## Therefore—an index of senses, ranked, grown without re-reading

### Entries are senses, positions are records, a rank says where to start

The shape is a subject index—library science's index of concepts, which need not appear as words in the text—with two changes: the position an entry points to is the whole record rather than a line—a sense rarely sits in one quotable line; it emerges from the record—and a significance rank is layered on so a reader with limited attention knows where to begin.

Senses, not words, is the load-bearing half. For example, in a CRM, churn risk almost never announces itself: one account's notes say the budget is frozen, another is "evaluating alternatives," a third's renewal call keeps slipping. Under the entry *churn risk*—described, never named—the index lists all three records; a search for "churn" finds none of them. A sense index exists to make exactly that connection.

The rank is the other half—take the teacher's Greek myth corpus as an example. The Hydra's venom runs through Heracles' story: he poisons his arrows with it, the arrows kill the centaur Nessus, and Nessus' blood, years later, kills Heracles himself. All three records sit under the entry *a defeated enemy's power returns*—and the rank marks the death of Heracles as the record where the sense lands whole.

Vector search is this design's nearest relative, and three departures define it: entries are discrete and human-legible, not points in a continuous space; each carries centrality, not just similarity; and the index answers with no model in the loop—it is a text file you can read, diff, and version like anything else you keep.

Two boundaries keep an index honest. Entries are selective—a lens's key senses, not everything sayable about the corpus. The record list under each entry is complete within what has been covered.

### A lens is a standing question, asked of every record

A lens is a standing question held against every record. For example, *cunning against strength: where, and how central?*—specific enough that "does this record answer it" has a yes or no. Your first lenses are the questions you have already paid for twice.

Its definition carries membership criteria, a few exemplars that anchor central against incidental, and its known blind spots. That text travels into every scan, so the judgment is repeatable across passes. A change of LLM may still bend it: prefer the same model throughout—and if you must switch, check what moved, or rebuild the index with the new one. For the lens above, Odysseus and Polyphemus is an anchoring exemplar: the whole record turns on wits beating force. Heracles' labors anchor the other end: force throughout, cunning in moments—present, and incidental.

The same machinery carries a business lens unchanged. Over customer meeting notes and CRM records, in a product whose main metric is NPS, a lens might ask: *what do customers name as driving their score, and how centrally?* New records arrive weekly, the question stands, and every re-ask is a lookup rather than a re-read.

Each lens keeps a register—its working table, one row per record, carrying the rank and the senses found there. The browsable index—sense → the records carrying it—is derived from the register mechanically, in one direction. Hand-edit the derived side once, and the two surfaces start drifting apart—every later regeneration either destroys your edit or preserves the drift.

Lenses multiply, and when they do they share one space. A boundary map records how adjacent lenses divide overlapping material—trickery in war could belong to *cunning against strength* or to a lens on *deception and its price*—so the division is decided once, not re-decided at every scan. And a lens added later is worth a full pass of its own over the corpus; it is the one cost the build's arithmetic does not cover. A keyword pre-filter, or a shortcut through records the other lenses already hold, might drop the records the new lens exists to find. A mis-drafted lens is repaired the same way—a fresh pass under the corrected definition; its old coverage does not transfer.

### Build with one read per record

The build is one read per record, serving every lens at once—cost scales with records, not records × lenses—and the read judges membership only, never significance.

The sequence is four operations:

1. **Define the lens**—question, criteria, exemplars, blind spots—before reading anything.
2. **Scan for membership.** One read per record, by the LLM you delegate the scan to—the lens definitions travel with it. For every lens: does it apply, and which senses does it carry? Write rows; assign no ranks. When in doubt, include: covered records are never re-read under the lenses that scanned them, so a missed sense is lost for good, while a spurious one is one row to delete when it next annoys you.
3. **Rank by comparison.** With the scan done, pass over the whole register and assign significance by a comparative question—*as central as the records currently at the top, or a crumb?*—never an absolute one. Absolute judgments made mid-read tend to inflate: with nothing to compare against, everything reads as important. On later passes, to measure the ranker's consistency instead of guessing it, seed the pass with a few already-ranked rows as hidden controls and see whether they land where they landed before.
4. **Assemble and derive.** Merge the ranked rows into the register, then regenerate the inverted index from it.

The first pass covers the batch you have, and coverage is recorded per record, so a partial pass is represented truthfully instead of rounded up to "done."

A register fragment from the teacher's lens—synthetic, like every example here:

```
lens: cunning against strength

record                     rank   senses
odysseus-and-polyphemus    ★★★    wits beat force · a name used as a weapon · escape by disguise
perseus-and-medusa         ★★     indirect attack · borrowed divine tools
heracles-twelve-labors     ★      force with moments of cunning
```

And the index derived from it:

```
wits beat force                → odysseus-and-polyphemus ★★★
a name used as a weapon        → odysseus-and-polyphemus ★★★
escape by disguise             → odysseus-and-polyphemus ★★★
indirect attack                → perseus-and-medusa ★★
borrowed divine tools          → perseus-and-medusa ★★
force with moments of cunning  → heracles-twelve-labors ★
```

How many rank levels you keep and what the top one means are yours to decide. The one property worth copying is scarcity: the top rank is reserved for the record you would start from, and the moment half a register wears it, it means nothing. That scarcity is also a stopping rule: open the top-ranked records, and leave the long tail of incidental mentions unread.

### New records fold in without re-reading the old

New records fold in by the same split, and the split is the whole reason the corpus can grow: membership is a local judgment, safe to make on the new records alone; significance is global—a rank means nothing except against the whole body—so only a pass over the complete register may assign it.

The failure this prevents has a general form: a global property assigned by a local pass drifts toward the fresh. A pass that sees only this month's batch finds everything in it important: freshness feels like centrality, and each append re-weights the index toward whatever arrived last. So the append runs in two layers—a membership scan over the new records alone, then a significance pass over the whole register, where the new rows compete against the full body rather than against each other. The pass reads the register, not the records—one line per record, so even a large corpus ranks from a small table.

A CRM example makes the failure concrete. The quarter closes and a batch of new records lands—a product change set off a complaint wave, and every fresh record reads as urgent. A batch-local read would rank the wave above the quiet records where the product's real drivers live; the whole-register pass makes it compete against all of them.

Three guards stand around the append:

- **A skew guard.** After each append, compare the batch's share of high ranks against the matched slice of the existing body—same sub-domain, same lens, never the corpus-wide average, which a genuinely dense batch will always exceed. A large divergence triggers a review, not a quota: demote what turns out to be incidental, and let an honestly denser batch sit above the average.
- **A vocabulary gate.** A new record may carry a sense your lens does not yet name. It either maps to an existing entry or waits in one adjudication list for a human decision—never straight into the register. That prevents a single batch from colonizing the index's language: the complaint wave would rename half your entries in the language of one incident.
- **Coverage by identity.** Coverage is recorded per record, under a name that survives the record being moved or reorganized—including the records that were scanned and matched nothing. The zero-hit case is the one naive coverage schemes lose: an unrecorded miss looks identical to an unscanned record, and gets re-read at every append.

However wide the membership scan fans out—several readers, several agents—the ranking of a lens is worth keeping in one hand, and so is the naming of its senses: split the rank judgment and the lens boundary blurs; split the naming and one sense grows two names—so at assembly, reuse an existing sense name before minting a new one.

Two slower rhythms complete the discipline. Every so often, re-rank a whole lens against itself: batch-by-batch appends accumulate small drifts, and a leveling pass sheds them without a corpus re-read—the register and the scan notes suffice. And watch the bottom of the table. When a class of new records keeps landing at the bottom of several lenses while sharing a sense the vocabulary gate keeps deferring, the index has discovered a missing lens—name the new question.

### Gotchas

- **Derivatives get a link, never a rank.** A synthesis or digest built from records already indexed may sit in the index as a navigation pointer—the one unranked thing the index allows—because ranking it would double-count every sense it borrowed from its sources.
- **Lens names can be more sensitive than the material.** Coverage and lens identity live on the index side only—never stamped onto the source records. A per-record "scanned under lens L" marker leaks the lens's existence to anyone who receives the corpus; kept index-side, the source stays lens-agnostic and shareable.
- **Index only settled text.** A record enters the scan when its text is settled—raw, half-processed material yields corrupted senses, and they sit in the register afterward as if they had been judged.
- **The corpus is assumed append-only.** Records arrive; none are edited in place. A live set of editable documents needs an adaptation this pattern does not carry—nothing here prices re-indexing an edited record.
- **Keep a registry of what is covered.** The index carries its own list of scanned record names, so finding what is new is a cheap diff of the corpus against the list—without it, every append starts by re-discovering what was already read.

### How you know it is working

The design makes one checkable promise—it finds records by what they mean, not what they say, and tells you which to open first—and the checks split in two: mechanical invariants cheap enough to run at every append, and sampled judgment checks that need a rater.

The invariants:

- **Coverage completeness.** Every scanned record accounted for, including the zero-hit ones.
- **Register ↔ index, both directions.** Every register row reflected in the index, and every index entry backed by a register row. A one-directional check passes a stale index, and passes it silently.
- **The skew ratio.** The append's high-rank share over its matched baseline, flagged past a threshold you calibrate on your own material.

The judgment checks:

- **Retrieval against gold.** Hand-label which records truly carry a handful of held-out sense queries, and measure the index against your labels. Weight the described-but-never-named queries heavily—they are where word search scores zero.
- **Rank calibration.** Have a rater order a sample of records under a lens without seeing the index's ranks, and compare. Falling agreement is the ranker drifting.
- **Append stability.** Re-run the significance pass over an already-covered slice. Ranks that move with no new evidence mean the ranking would not survive its own repetition.

Which of these to run, and at what scale, depends on your corpus—these are shapes to adapt. The cheapest one needs no apparatus at all: pick a sense you know lives in the corpus, and see whether the index alone takes your agent to the right records—no search, no re-read.

### When not to build one

Skip it when the whole corpus can be cheaply re-read for every question, when you want the words themselves, when you will read it once and never ask again, or when you want the meaning told rather than located—each has a cheaper instrument.

- **Search—lexical or semantic—** is better when you want occurrences: the words themselves, or a quick neighborhood of similar passages. Either coexists with a sense index—search finds where something occurs, the index says where it lives centrally—and neither substitutes for the other.
- **Tags** are better for small corpora and literal categories. A controlled tag set drifts as the corpus grows, carries no rank, and cannot express a sense the text describes but never names.
- **Vector search, and the RAG stack around it,** is the default answer at scale—and it may solve your problem outright, possibly better than this index will. Below that scale, this is the hand tool.
- **A written synthesis** is better when you want the story told. It cannot be queried, it goes stale silently, and one distorted record can bend the whole account. The index degrades more gracefully: a bad record is one row.
- **Summarize-on-demand** is better for a true one-off. It re-reads everything on every ask—the failure the ranking discipline above exists to prevent.

Build one when the same records are worked by session after session—the questions keep coming, the records keep arriving, and nothing read yesterday is remembered today. The index is for the asker who returns.
