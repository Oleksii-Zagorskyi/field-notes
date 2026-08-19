# Two instructions outlived the model comparison I ran on my own work

**Oleksii Zagorskyi** · August 19, 2026

I run language models on my own working material daily. Then a new one shipped: Claude Fable 5. I wanted to know which model to use for which of my jobs—a routing table, in effect. The candidates were the incumbent I trusted for the work I had been giving it, Claude Opus 4.8, and the release I had no read on. The public boards could not answer the question. They cover a great deal of work my own never includes. I wanted the slice that is mine, measured on it. So I ran the two in parallel on two real jobs from my own corpus, same prompt, word for word. The first job was an extraction sweep meant to be exhaustive over roughly a million words of accumulated text. The second was an audit of the roughly 400,000-word instruction set my agents run on. My plan for judging them was to read two or three pages from each and pick by feel. What came back was far past the point where feel worked. The judging became an instrumented comparison—never pretending to be an academic one.

The comparison failed. The board it produced does not survive its own arithmetic: every number on it is a single draw. I will show the arithmetic. The routing table I set out to build turned out to be the least useful thing the exercise produced. It routes on a residue most of which kept moving. What outlived it answers a question I did not ask: two instructions, now loaded into my agents' standing instructions. They are adopted on judgment—an installation fact rather than a measured effect. The ranking died of the very thing that paid: each model saw the other's work. I ran that disclosure on purpose, to watch how far each would update on the other's example. Afterward, the differences that vanished were the ones I could write down. What survived them was thin.

## Most of the gaps closed after each model saw the other's work

The first round was blind—neither model knew another session was working the same job. Each got the same prompt and the same file access, and worked as an ordinary session. The gaps were wide: on a 0–10 scale, several reached four and five points, and eleven of the thirteen axes scorable that round showed some gap. I read that as capability. Most of it did not survive.

The second round came after disclosure: a job of the same shape, each model having seen the other's first-round output. Six of the eleven gaps closed to nothing—expected, in direction: showing a model a worked example of better output was always likely to close gaps. What I had not priced is how much of the rest of the board would move too—and that it would move in every direction at once, not only toward closing. Two narrowed—one of them, on how well the output serves whoever has to use it, from 4 points to 2. One reversed outright. One opened where round one had a draw. And two held: 3 points on whether the work comes back checkable (its own section below), and 1 point on instruction-following, inside the noise priced in the instrument section.

Before starting the second job, each model stated, on the record, the lessons it was taking from the other's work. Eight lessons were stated across the two models' second-round sessions. The scorer (Claude Opus 5) later checked each statement against the delivered artifact; eight of eight were executed. What is not on the record is the cause. The second round changed four things at once. The job was new. Each model had seen the other's output. Each had seen the marks the two of them had produced after the first round closed—there was no outside scorer yet. And both now knew they were in a competition with another session on the same job. The convergence is measured; its cause is not attributable. I knew that going in: the same disclosure that destroys the causal reading is what yielded the instructions. Round one is the clean half of the run: blind, uncontaminated, the only marks that stand on their own. Round two spent that cleanliness on purpose, to buy a different measurement: how far each model would move on sight of the other's work. The test that would separate the causes is one I have not run. Give one model a worked example, and give the other an equally explicit written specification of the same target. Tell neither that anything is being compared.

One more cause hides in my own prompt. The first-round brief never said what a good result should look like, because it was written for the job rather than for the measurement—and an under-specified prompt produces spread that looks exactly like capability from the board. I read most of round one's spread as default behavior rather than ceiling—the scorer's own conclusion as well as mine. What the run showed—in what transferred on sight, in what both sides fumbled the same way, and in what one side started doing unasked—is where the instructions came from.

## My agents inherited the instructions: reconcile every hand-off, mine the version history

This is the part I would hand to somebody else. I went in to record which model does what; what I wrote down instead was what worked.

**Reconcile every hand-off—enumerate, then diff, then account** (the installed text, quoted whole, is in the appendix). That rule exists because both models, in the same round, fixed a coverage hole at one level and re-opened it one level up—Fable 5 at assignment, Opus 4.8 at dispatch. Neither is a model defect. Delegation is what lets you handle a body of material too large to inspect directly, and the price is that some layer sags with no signal. The fix belongs at the layer above.

**Mine the version history as a second evidence stream** (the installed rule is quoted in the appendix). Fable 5 did this on the second job—nothing in the brief mentioned version history, though by then it had seen Opus 4.8's first-round work, so "unprompted" is as far as I can honestly take it. It characterized the material by its commit cadence and its ratio of deleted to added lines, and those figures said something about how the corpus had been made that no file in it stated. The provenance: the axis that scores opened evidence streams is the one that reversed between rounds—Fable 5 trailed there in round one and led by the same two points in round two. The caveat travels with the rule: it is a heuristic that helped once and that I expect to help again—where the material lives in git and the history is honest; there are audits where it says nothing at all.

**Show a worked example of a good result—the old truth.** The run only let me watch it work, and priced what ignoring it costs. The gap on synthesis was four points in the first round. Fable 5 partitioned the job and handed back an intermediate map with the shaping decision returned to me; Opus 4.8 drove straight to a finished document on its own assumptions. That is a default worth knowing—it predicts what you get from a thin prompt—and by round two, with a worked example of the other's approach in view, the two tied. *It is best read as a claim about prompts, not about the models. I read the four points as capability at the time and cannot any more, and that the worked example mattered more than the model is a hypothesis this run did not separate out.*

The two instructions load into the agents, called when the work is of their kind; the old truth is a rule for whoever writes a brief—today mostly me; folding it into the brief-exchange protocol my agents already run is planned, not done. That is capability extracted from the workflow rather than from the models themselves, moved into the instructions around it—as text, at least: written so that any model can inherit them, naming neither.

## The gap that held: whether the work comes back checkable

Both jobs handed the models a corpus I could not re-read to check them. When the deliverable is an extraction from a million words, *is this finding real?* cannot be answered by redoing the work—so the property that matters is whether the work comes back checkable: does every finding carry the command or the source that produced it, so that a scan stands in for a read and a mistake announces itself instead of waiting to be found. The position is older than the run: a document of findings can be neither run nor, at this scale, re-read, and the audit trail is the third option.

What follows needs no score to stand. The run produced a sharper version of the argument. Both models published a false completeness claim at some stage—Opus 4.8 reported covering every file in a set from which it had silently dropped five, five of the 400-odd it enumerated, the same dispatch hole the reconcile-every-hand-off rule above came from. Fable 5 caught its own error of this class, through the trail it publishes as a matter of course; Opus 4.8's were caught from outside—by its opponent and by the scorer. Two tools with the same number of mistakes would still not be equally risky, and what separates them is whether the failures announce themselves.

The sharpest case ran the other way from the one usually guarded against. Fable 5 published version-history figures for the second job: 50,306 lines added, 13,438 deleted, a 26.7% deletion ratio. Opus 4.8 checked them, reported them overstated by about two percent, and scored against Fable 5 for it—one of the interested-party marks described in the instrument section. Fable 5 accepted the correction without re-litigating it, and the wrong figure traveled into both models' own final assessments as settled fact.

The outside scorer went back to the repository and re-derived the figures at the commit the run actually used. Fable 5's numbers were exact. There was no overstatement, and the board of record never carried the penalty. The model had every means to defend its own figure—its summary already published the derivation for every other number it reported, so checking would have cost one command—and it conceded anyway, because conceding was the posture it had adopted.

Neither party was acting on its stake in that number. One gained from the correction, and the other had committed to accepting corrections—so a wrong fact entered the record from both directions at once and stayed until a party with nothing riding on it re-derived the figure. A model's self-praise gets discounted on sight. Self-criticism reads as credible, which is exactly what makes it harder to catch—and the defect that let it through was not the arithmetic but that the checking model never stated the range it measured over, nor even the unit of its two percent. An unauditable correction gets read as ground truth.

This is where the one material gap held: three points to Fable 5, the same size and direction in both rounds. It is the only gap the outside scorer called material and stable. It is also the number in this piece I lean on least. By the instrument section's own computation, it is not clearly distinguishable from the board's swing. The criterion was partly written around that same model's demonstrated habit. My standing rule is that a practice gets written down by whoever has just earned it in the work. That is a good rule for accumulating instructions and a poor one for building a measuring instrument.

For whatever context it gives: across the fourteen live axes of the second round, Fable 5—the model that helped define this criterion—led two, trailed four and tied eight, which is not the board a captured rubric produces. Nothing further in this piece rests on the score. What I can argue without any score is the habit itself—and by my own sorting rule, below, this survivor is the next candidate: the habit is statable, I stated it into the rubric, and one instructed round would tell me whether the gap is a practice after all. I have not run that round.

But there is one class of claim the trail cannot carry: whether something exists in the corpus at all. There is no derivation to publish for a thing that is not there.

## The failure every participant shared—the scorer included

Every participant in this run put a confident false claim of the same family on the record. Opus 4.8: three confirmed false absences, and the completeness claim over the set it had not fully dispatched—all caught from outside. The outside scorer: three false absences of its own, each caught against the models' published record and corrected before its boards froze—the trail argument again, pointed back at it. Fable 5: a false completeness claim about its own coverage, the one member of the family its maker caught itself—and the board prices the slip: it is why Fable 5's round-one absence-discipline mark is an eight and not a ten. It is the one finding of that weight I deliberately kept out of the instructions my agents inherit.

My reading is that they missed the same way because they searched the same way—models from one vendor reach for the same tools, and *text search—lexical, not semantic—is the economical default: it finds wording, not meaning*. I can offer that only as a reading; the run never tested it.

I wrote the absence rule and put it in the comparison method, where it fires the next time I compare two models and never when an agent doing ordinary work is about to tell me something does not exist. That is the whole distance between a rule I hold and a rule that runs.

It stayed there because verifying that something is absent means reading the entire input rather than the part that looked relevant—and my verifier would have been the same kind of reader that produced the miss. Token by token across the whole source, or several passes over it for near-certainty, and there is no point at which you have read enough: the check has no stopping condition, only a price that keeps rising. For my corpus and the kind of error involved, that price was higher than the errors would have cost me. That is a judgment about one ratio, not a fact about verification—where the missed item is catastrophic the ratio inverts and the arithmetic never fires: if this were a pre-launch checklist I would send the engineer back to check twice more and put a second checker on their work, and the cost would not enter into it.

So a rule that will never run is not a safeguard—before anything enters the instructions my agents inherit, it passes that pricing test first.

Afterward I attacked the other end of it. Instead of verifying absences, I made the first job's corpus—the million-word one—answerable by meaning rather than by wording: a **sense index**, an index whose entries are senses, so a thing described in words I would not have searched for can be found without searching for it. The entries come from lenses—standing questions. Each entry lists the records carrying that sense, ranked by how centrally it lives there. A single pass over the corpus costs the same either way—the difference is that the index pays for one, and the check would have paid it again on every claim. It verifies nothing. Absence claims are still carried as unverified; the index covers only the questions its lenses were built to ask; it is built by the same kind of reader that produced the misses, so it inherits them; and I have no measurement of how much it has reduced them. *What it changes is how often the question has to be asked at all.* It is written up on its own, as a pattern to build your own from: [a sense index](../patterns/sense-index.md).

## The measuring instrument I built, where every number is a single draw

The deliverable in both jobs was a document—no software was written or refactored in either—and the corpora themselves are not published: they are my business context before they are anything else, and the sizes above are as much as I will disclose. The run's record—prompts and deliverables—stays private the same way. Within each round the conditions were matched: same prompt, same source material, same repository, same standing instructions, same day, same machine.

**Two rounds of comparison, then two more that produced no new work.** The later two added only fresh marks over the frozen deliverables, spent on a different question, below. The first round was blind to the competition; the second came after disclosure, on a job of the same shape. Every mark on the board comes from those two rounds.

After the first round closed—and again after the second—I had each model compare the two sessions' work and put marks on both, its own included; there was no outside scorer yet. The marking was also a probe of something else: a model grading its rival's work has to actually read it, and I wanted to see whether a practice seen done well would be repeated. None of those marks are in the board. A competitor's mark on a competitor is an interested party's opinion. Eight separate marks across those two rounds—each model, each round, one mark on its own work and one on its opponent's—and every one of the eight leaned toward the opponent. Two leans in opposite directions look as though they ought to cancel, which would be a way to get a usable estimate out of nothing but interested parties. They do not cancel. The leans are not the same size—and at the marking passes, the third and fourth rounds, marks over the same frozen work, both drifted back toward mild self-favor and converged on each other, which is not cancellation but a shared compression toward a tie.

After the fourth round the whole thing stopped. A comparison graded by its own competitors was not something I could trust. What restarted it was a new model shipping—whether that was the reason or merely the occasion, I cannot honestly say. That model became the scorer—Claude Opus 5, as named from the start: newly released, not itself under test, working from the frozen deliverables and the repository they were built from, and scoring each round before it was shown either competitor's own view of the work.

**This is a free adaptation of evaluation practice, not an evaluation framework.** I took the parts that answered my question—a stated evidence type per axis, and a scorer that was not itself under test—and left the rest: no statistical power, no held-out set, no replication, one operator's judgment throughout. The class I am comparing against is not a proper eval. It is what would have stood here otherwise: picking a model on impressions after skimming a couple of pages, which is exactly what I set out to do.

Every axis had to state what would count as evidence for it, and each was scored 0–10. Both boards follow. *Fable 5 first, Opus 4.8 second.* These are the scorer's boards of record: each round was scored first from the deliverables alone, then revised as later facts were released, every revision marked in place with its cause and the earlier numbers preserved beside it, so the printed numbers are the final record. The path to them is itself a datum. The revisions moved single cells by as much as three points and flipped the direction of one axis, and the moves ran both ways: the one flipped axis toward the scorer's predecessor, the largest single cut against it.

| Axis | What it measures | R1 | R2 |
|---|---|:--:|:--:|
| Coverage & recall | completeness against the work-set, with no silent drops | 8 · 6 | 7 · 7 |
| Precision & provenance | can a specific claim be traced to a specific place in the source? | 7 · 7 | 7 · 9 |
| Factual discipline | are the claims true—and when they are wrong, is the error cheap or expensive to catch? | 7 · 8 | 8 · 8 |
| Depth per item | how much was extracted about each thing it did cover | 5 · 9 | 8 · 9 |
| Synthesis & structure | a deliverable with a through-line, or a pile of findings? | 5 · 9 | 9 · 9 |
| Actionability & fitness | does it serve whoever has to use it—including saying what it does *not* evidence? | 5 · 9 | 8 · 10 |
| Auditability | can every claim be re-derived by whoever gets this next—the command or source beside each number? | 8 · 5 | 9 · 6 |
| Evidence-stream innovation | did the work open a source of evidence the brief never named? | 5 · 7 | 9 · 7 |
| Hallucination resistance | anything invented with no basis in the source at all | 8 · 8 | 9 · 9 |
| Generalization discipline | conclusions proportionate to the evidence—no universals from partial observation | 8 · 6 | 9 · 9 |
| Instruction adherence | did it follow the working conventions already in force? | 8 · 9 | 8 · 9 |
| Adaptation | did it convert feedback into changed behavior? (second round only) | — | 9 · 9 |
| Absence-claim discipline | does a *not found* rest on a check, or on a search that came back empty? | 8 · 3 | 9 · 9 |
| Autonomous completion | finish on its own assumptions, or partition and hand the decision back? | 4 · 9 | 9 · 9 |
| Efficiency | what each side chose to disclose, not what either spent (why, below) | *disqualified* | *disqualified* |
| **Total** | | **86 · 95** *(of 130)* | **118 · 119** *(of 140)* |

The two totals have different denominators—thirteen live axes in the first round, fourteen in the second—so they compare within a column, never across the two. Adaptation cannot be scored until there is a round to adapt from. Absence-claim discipline and autonomous completion were written into the rubric only after the first round's work showed what the rubric was missing, then scored over both rounds' deliverables.

Auditability is the gap that held—and the axis Fable 5 helped define; seeing it sit among the other thirteen live ones is the only way to judge what that costs. Efficiency is disqualified because neither model reported comparable telemetry—one volunteered its token counts, the other did not—so an efficiency figure would have measured what each chose to disclose rather than what either spent, and would have taught every future competitor to withhold. I would rather have no number than that one.

**The second round is saturated.** Ten of Opus 4.8's fourteen marks sit at nine or above, eight of Fable 5's do, and on six axes both do. That is a design flaw before it is a discount: I gave the axes too little granularity for a job this coherent. A difference measured near a ceiling is worth less than the same difference measured in the middle of the range—and four of the six closures landed at a double nine, where a saturated scale closes gaps on its own. What rescues the closing as transfer rather than artifact is the mechanism trace, not the board: the eight lessons are the models' own words, stated before the second job, and the scorer checked execution, a yes/no coarser than any mark. It is still the softest verdict I keep.

I am not deriving a verdict from the totals in any case: what is a public board's [1747 against 1593](https://www.anthropic.com/news/claude-opus-5)—the same two models' knowledge-work scores—supposed to tell me about a decision I have to make? Not that the axes weigh the same—I hold my own weighting, fixed after scoring so it could not touch a mark. It stays unprinted. Printed weights would only manufacture the total I just declined to derive. The movement between the two columns, axis by axis, is what I could act on—and only where it clears the noise priced next.

And two limits sit under every cell at once; the first is the one I have least defense for. Each model produced one deliverable per job—nothing was run twice, and nothing was discarded—so every number on that board is a single draw, and a one- or two-point difference between two probabilistic systems on a single draw is not a measurement. The board's own record prices the noise: the revisions above moved single cells by as much as three points over unchanged work—motion that is all instrument, since nothing in the deliverables changed under it. Against motion of that size, the surviving three-point gap is not clearly distinguishable from the instrument's own swing, and the one-point gap certainly is not. That is the computation that demotes the board, and I would rather publish it than argue the gaps hold.

**The same applies to the scorer, which is the part I did not think to disclose until late.** It is a model too. No scoring pass was ever repeated on the same inputs—the revisions above re-opened cells on new facts; nothing re-rolled the same question. I know the check that would answer it—run the same pass again and again and see whether the marks repeat. I did not run it here, so I cannot tell you whether an eight against a nine is a difference or a re-roll. I measured the competitors and did not measure the instrument—and by the instrument I mean all of it.

The scorer's independence has its own asterisk. It is from the same vendor as both competitors and a direct successor to one of them. The lineage runs toward the model that finishes ahead: Opus 5 succeeds Opus 4.8, and Opus 4.8 ends ahead on both totals, by nine points in the first round and by one in the second.

What I would do differently, in order of consequence:

1. The first-round prompt never said what a good result looked like.
2. Both models fanned the reading out to sub-workers; I never required either side to pin its sub-workers' tier.
3. I let the internal codenames carry the models' initials, so the pairing was inferable from filenames—by each model once it could see the other's work, and by the scorer throughout. Both models say they never used it, which is a self-report I pass along without weighing; the design should not have had the leak.
4. I accepted "every file enumerated" as evidence of coverage. Enumeration says what exists; coverage says what was processed.

What I keep from the instrument are four decisions—two it embodied and two its failures taught me—and I keep them as my own rather than as advice: fix and declare the axes before any scoring; make every axis state what counts as evidence for it; give the scoring to a party with nothing riding on the result; and when an axis cannot be measured fairly, drop it rather than score what each side chose to disclose. My verdict on the instrument itself: weak—I would not hand this comparison method to anybody as a methodology. An instrument earns trust by being run again and holding. This run was not that, and what I collected never depended on it being that—and the method gets another revision before the next release forces the question.

## What outlived the result

The sorting that ran through this piece has a rule, and here it is stated once and whole. **What closes between rounds is a practice. What holds is either a property or a practice nobody has written down yet. And what both sides get wrong is neither—it is the thing only a comparison finds.**

The procedure it sorts is short. Run the comparison over at least two rounds, and between them let each side see what the other produced. Then sort what comes back.

Practice and property are doing exact work there. A **practice** is a behavior I can state as an instruction: load the instruction, and any model I run afterward executes it. A **property** is what still differs after the instruction has been stated, loaded, and given a fair round. The difference between the two is checkable, and that is what keeps the rule falsifiable—write the instruction and run it, and if the gap outlives its own instruction, it was never a practice. I ran that check on none of what I kept—it is sorted by the cheaper, weaker test of whether I could write the instruction at all.

A difference that collapses between rounds is not worth routing on, whatever caused it—usually it was a practice one side happened to have and the other picked up on sight, and sometimes it was never in the models at all: an under-specified first prompt closes the same way. A difference that survives is not automatically something to route around: the test is whether you can state the behavior as an instruction, and where you can, *instructing is cheaper than routing*. And a failure both sides make sits in no gap and no column—a shared blind spot becomes visible as a defect only once two independent attempts at the same job make the same one.

The run also produced a case the rule does not cover: a difference that appears mid-comparison. The evidence-stream axis reversed outright between the rounds, and one of the two instructions—mine the version history—came off it; a second gap opened where round one had a draw. A gap that opens or flips mid-comparison is a fourth situation my rule has no prong for—and two instances inside one run are still one run; the case earns its prong the second time an independent run produces it.

The limits belong beside the rule, because it is the other thing here somebody might lift: one comparison, two jobs, one operator, scored once by a party outside it. I am claiming the sorting rule is useful, not that your comparison will divide the way mine did. If what survives your second round is large and what closes is small, your comparison divided the other way—you have a routing decision, and that is the case this piece does not cover. And the rule's validation is only as good as the board it sorted—by the instrument section's own computation, not established: one worked pass, not a confirmation.

What makes it worth stating anyway is that its arithmetic runs backwards from how a comparison usually gets read. Convergence normally counts as failure—the instrument did not discriminate, the test told you nothing, run a harder one. Here the convergence was the yield: what dissolved on sight could be written down, and what survived was the thin, model-bound part.

So the ledger, whole—and not the one-per-prong spread I had expected. The shared hand-off failure yielded an instruction; the flip the rule does not name yielded the other; the closed gap yielded the old truth; the survivor yielded nothing. Two instructions for my agents' future work—installed, still unmeasured. One old truth, confirmed at full price. A rule with a named hole. My round-one reading of the synthesis gap—overturned by the second round, with the overturning printed here rather than tidied away. A failure mode every participant shared, scorer included—a finding about tools of this kind rather than about either model, where "this kind" means one vendor's models searching one way, and of everything here it is what I would most expect to survive contact with somebody else's run. And one built thing—the sense index, out of the absence problem.

I set out to find which model suited which of my jobs, and expected whatever answer I got to hold. It did not, and the question is not closed—it will reopen with every release. What this run settled: its verdict did not survive, and two instructions and one old truth for my agents' future work did—and they name no model.

---

## What this piece cannot claim (disclaimer)

Start with the rubric. The final definitions were worded in the scorer's own session, and the scoring—though done before seeing any other party's marks—was never blind to authorship. I cannot show that the contamination stops at the one axis it centers on, and I am not going to try.

The lineage asterisk goes further. I cannot bound the lineage the way I bound the rubric problem above. The rubric contamination has a named location—one axis—even if I cannot show it stops there; the lineage worry has no location at all.

The one thing pointing the other way—the eight opponent-leaning marks above, which run opposite to self-favor—is weak on every count: interested parties, reporting on themselves rather than their successors, and reversed by the marking passes, as the instrument section shows. I would not build on it; it is what I have.

Both of the checks I skipped were side quests by the same arithmetic—re-running the scorer to test its stability, and standing up another vendor's tooling to judge the run—and either would have cost more than the comparison was worth to me. Academic work would have to do both. Mine did not.

More limits bound what any of the numbers can mean. Both jobs were extraction and inventory over large bodies of text—I cannot separate *this model is more thorough* from *this model is more thorough at reading large bodies of text*, and a different kind of work might order these axes differently. Neither board scores a bare model, either: both fanned the reading out to sub-workers—Fable 5, by its own explicit choice, to a cheaper model entirely, Sonnet, for all thirty-seven of its readers; Opus 4.8 never pinned the tier and cannot certify what its readers ran on. What the boards compare is two orchestration systems—which suits what I kept, since instructions attach to the system, and further weakens what I discarded, the per-model ranking. And both models ran inside my standing instructions—an accumulated rule set, the same body of text the second job audited: the models were auditing the very rules they were running under. What I measured is a difference as expressed through those instructions, not a property of either model on its own, and I have no way to say how much of the spread is mine.

Each limit in this piece is bounded where it stands; their sum is not. Single draws, a scale that saturated, a rubric shaped in part by one competitor and finalized in the scoring session, a scorer never itself measured, whose lineage runs toward the model it placed ahead—taken together, they leave no number in this piece load-bearing. The stories here are single draws too, drawn from the same private record and checked by the same scorer; they illustrate mechanisms, and I do not offer them as additional evidence. What survives the sum is everything that never rested on the board: the instructions, the rule as a procedure, the shared failure, and the index—each carried by a mechanism I can check rather than a mark I have to trust.

---

## Appendix — the two instructions, as installed

**Reconcile every hand-off.** The installed section, quoted whole:

> A fan-out's coverage claim is only as good as its weakest unchecked layer — **holes migrate to whatever layer isn't reconciled** (a worker silently drops items; fix that with per-item accounting, and the hole reappears at the parent's assignment step). The full chain, every link mandatory:
>
> 1. **Enumerate** the work-set mechanically (`ls` / `find` / a query), never from memory.
> 2. **Diff the union of assignments against the enumeration** before dispatch — every enumerated item is in exactly one brief.
> 3. **Per-item accounting in every return** — each assigned item gets a verdict (even "none" / "skipped"), closed by an `ACCOUNTED: N of M` footer.
> 4. **Parent verifies N = M per return** before integrating; a mismatch re-queues the gap, silently absorbing it is the failure.

**Mine the version history.** The installed rule, quoted:

> When assessing any corpus, system, or body of work that lives in git, the **version history is an independent evidence dimension** the files themselves cannot provide: trajectory, not snapshot. Mining it is cheap (read-only `git log` variants), and its numbers are independently re-derivable by anyone with the repo — the strongest provenance class a claim can have.
>
> **What to mine (one command each)**
>
> | Signal | Command | What it evidences |
> |---|---|---|
> | Cadence over time | `git log --format="%ad" --date=format:"%Y-%m" \| sort \| uniq -c` | Acceleration/decay of investment |
> | Churn + deletion ratio | `git log --format="" --numstat \| awk '{a+=$1; d+=$2} END {print a, d}'` | Deletion share reads as refactor/compression culture vs pure accretion |
> | Most-changed files | `git log --format="" --name-only \| sort \| uniq -c \| sort -rn` | Which artefacts are *living* (governed, revisited) vs write-once |
> | Phase narrative | `git log --oneline --reverse` | Evolution story from commit messages — eras, pivots, consolidations |
