# Eliciting intent—an agent that gets to the bottom of what the owner means, not just what they have said so far

**Oleksii Zagorskyi** · October 28, 2026

*This is a pattern for an agent that interviews whoever holds an intent (you, or someone you build for) until it is a document they would sign. What follows is the practice's shape, and the reason for each part of it. Give it to your agent to build its own version of this practice.*

Eliciting intent is a practice for interviews in which an agent draws out what the owner—whoever holds the intent and decides—means, and writes it down as a document they would sign. It exists to prevent one failure: questioning that stops short, leaving part of the intent in the owner's head and the document as they first drafted it. This article follows one example, a request from the head of a sales team:

> **Owner** — "We need an automatic pipeline that rates incoming lead requests from urgent to just screening tech specs, gives urgent and medium to a senior sales manager, low priority to a junior one, and puts just screening in the backlog."

Everything in it is true, and it is incomplete: it names a solution without saying what goes wrong today, its four ratings have no criteria, and it describes only the case where everything goes right. The agent's first rounds on it appear below. The interview pays off when the owner will act on the document or approve it, and judges that an incomplete one would cost them more than the rounds of questions.

## When someone needs their intent written down as a document they will stand behind

This practice fits when one owner, in a conversation with the agent over as many rounds as it takes, holds an intent they will act on or approve once it is written—a vision, a plan, a specification, a negotiating position—and judges that it is not yet fully in words.

## An agent settles on the first picture that hangs together, before the owner is asked what it leaves out

Asked to clarify and then write, an agent left to its defaults tends to stop asking once what it has heard hangs together, and writes that down as the owner's intent. The document then stays as the owner first put it, and whoever builds from it comes back with questions, or improvises.

## Therefore—the agent leads the interview in rounds, keeps the record and pushes back; the owner decides, and nothing goes into the document until it is settled

### The interview walks the decision graph from the owner's aim—first the questions others depend on, then the document's outline, then the details—asking each question once what it needs is settled

Each question the work raises needs some others settled before it can be answered; that is the decision graph. The agent walks it from the aim, through the questions others depend on, then the outline, down to the details, the questions no other question needs. It does not draw the graph up front: each question carries what it needs, written beside it, and the graph grows round by round from what the last round settled. Back to the sales team's request. The agent first looks up who is on the team (two senior managers and two juniors, one of them on call after hours) and, in the CRM, what it means to assign a lead to the person responsible, and where and how that is done, rather than asking. Then it asks in rounds.

> **Agent** — *Round 1: the aim*
>
> - **q-1** What goes wrong today without the pipeline?
> - **q-2** How would the team know, a month in, that it worked?
>
> **Owner** — Hot leads sit in the shared inbox for a day or two and go cold. A month in, no urgent lead should wait more than an hour for a call.
>
> **Agent** — *Round 2: the ratings, built on the aim.* If I read you right, urgent is about speed to the first call—is that so?
>
> - **q-3** Given that the point is speed to the first call, are urgent, medium, low and just screening the whole scale?
>   - (a) yes, those four **Recommended**
>   - (b) add a level
> - **q-4** What made the last urgent lead urgent?
>
> **Owner** — Yes. q-3 a. The last one had a budget and a date this quarter.
>
> **Agent** — *Round 3: the edge cases, built on the ratings*
>
> - **q-5** A lead meets the urgent criteria but arrives after hours:
>   - (a) urgent now—the on-call manager calls within the hour **Recommended**
>   - (b) first thing in the morning
> - **q-6** The senior manager has no capacity left:
>   - (a) pass it to the junior, so the call happens within the hour **Recommended**
>   - (b) escalate to the head of sales
>   - (c) something else—say what
>
> **Owner** — q-5 a, q-6 a.
>
> **Log** — *D-6* (settles q-6). When the senior manager has no capacity left, an urgent lead goes to the junior, who calls within the hour. *Alternatives:* escalate to the head of sales. *Needs:* D-2, a call within the hour; D-4, what makes a lead urgent.

Each round is built on the answers to the last: the scale waits on the aim, and the after-hours case on the scale. The aim's questions are open-ended; each edge case is its own bounded question, with its options and one of them recommended. The owner's answers shorten round by round, down to two letters. That is a sign, not a proof, that this part has settled: an owner who only accepts the recommendations answers just as briefly.

1. **Rounds by dependency.** The agent asks in rounds: a round holds every question whose needs are settled; one that needs a question still open waits for the next round. A bounded question carries its options, one of them recommended, and the owner can answer with a letter; an open-ended one carries no options. Without it, the owner can answer a question that a still-open question makes moot, and the answer has to be reshaped afterward.
2. **The aim first.** Before any solution, the agent asks about the aim—the problem the work serves, and how the owner will know it worked. An aim the input states is not taken as decided: where its wording is vague, the agent offers sharper wordings, the recommended one first, and the owner confirms one or refines it. A solution the owner names is traced back to its aim. The aim alone is never held open or pruned: until it is decided, the interview does not move past it. Where nobody names an aim, the agent proposes some drawn from the input; if the owner takes none and names none, the interview ends, and the agent hands over what was said, the aims proposed and why it stopped, since without an aim every later question spends the owner's time on a target nobody has named. An interview that skips the aim or leaves it for later can produce a precise record of the wrong thing.
3. **Past the first answer.** The agent takes the first statement as true and incomplete, and reads every statement for what it leaves unsaid: the cases a happy path leaves out, a solution named without its reason, a vague word without a test. The drawing-out is done when nothing is left to draw out of what is recorded and the answers have stopped opening (property 8). Without it, part of the intent stays in the owner's head, and the log holds only what they had put into words.
4. **The owner decides; the agent recommends, records and marks its readings.** The agent recommends an option in every bounded question and records what the owner chooses; the owner decides what to settle, what to explore and what to leave. A branch the owner declines—a question and the questions that need it—is recorded as pruned, and the agent does not reopen it; a question they are not ready to answer is recorded as held open, and the agent does not press it. What the agent infers is marked as its reading, never written as the owner's. Where these roles blur, the agent's synthesis can be recorded as the owner's will, and the interview can dig where the owner chose not to go.
5. **A decision log first, the document from it.** The agent writes each decision to a decision log as it settles—a full sentence, its alternatives, and the numbers of the decisions it needed—and each open question goes into the question register the turn it is asked. Each entry points to the entries it rested on. That is how the log keeps the graph's direction, and why it is both the interview's audit trail and its graph; the conversation can resume from it. The agent writes the document only from the log, one cluster at a time (a cluster being the questions about one part of the work). Writing starts once the aim is decided and the questions others depend on have an outcome, from a skeleton of the document's sections, or from the document itself where one already exists. The skeleton and each cluster's summary come with the next round, and the owner confirms them with a word or corrects them. Without it, decisions can live only in a scrolled conversation, or the document can be rewritten after every answer while its foundations move.
6. **Pushback before writing.** To push back is to stop an answer before it is written, name what it pulls against (quoted where it is written down), say what writing it as stated would do, and ask a bounded question whose options tell apart what the owner may mean, one of them keeping the statement as said. Pushback ends in a recorded decision, where a clarifying question ends in information. The agent pushes back wherever an answer would:
   - pull against what is already said or settled;
   - carry nothing for what the document is for, or turn the discussion away from its aim;
   - work against the aim it is meant to serve;
   - rest on ground nobody has checked.
   
     In each case, the owner, not the agent, decides whether it stays. Among the rules of thumb at the end (heuristics for particular situations) are one or more for each case. The agent records a confirmed change as a decision that supersedes the old one, which stays in the log; that is also how a closed part reopens. An answer written without pushback can override, by accident, a decision the owner has forgotten, and leave the log contradicting itself.
7. **The close.** When no question is left to ask, every topic the owner raised maps to one of four outcomes—decided, deferred until a named event makes it answerable, pruned, or held open—and the agent reads the log back, one line per decision, each traced to where the document says it; the owner approves the document itself. Without it, a topic raised early can disappear, or the document can drift from its decisions, unnoticed until it is used.
8. **The length of an answer.** An answer that runs long where the letter of an offered option would have been enough is intent still opening: its new edges become the next round's questions, and the interview does not close while answers are still opening. Without it, new intent can be read as noise, and the interview can close while it is still opening.
9. **An answer authorizes what its question proposed—no more.** The agent proposes other work an answer unlocks—a new kind of document, an edit outside the work's files, a deletion—as its own step. Without it, a "yes" to one question can become permission for work nobody asked for.
10. **Check before asking.** The agent checks for itself any fact that the files, the log, a web search or a tool can answer, and asks the owner only for decisions and for what only the owner can do. The agent hands a search too large for the conversation to a helper agent, where that is worth its cost. Without it, the owner's attention is spent on what the agent could have seen.

Each round costs the owner one reading and one answer (a line, when the questions are well shaped); each cluster, one summary to confirm; the whole interview, one read-back and one approval. The number of rounds follows the intent, and is not fixed in advance.

The heuristics come in three families, given whole in the appendix: Grounding keeps the record true, Shaping asks each round right, and Polishing keeps the exchange easy. Without Grounding, the decisions written are wrong; without Shaping, the questions answered are the wrong ones, or come in the wrong order; without Polishing, the owner works harder and the record loses their voice.

### How you know it is working

The **practice is worth it** if, for intents of the same kind, its document leaves fewer questions for whoever uses it downstream, and fewer topics dropped, statements corrected, or statements disowned, than a document written without it.

To test it, run a paired trial on comparable pieces of work, each one owner with one intent, taken in pairs: the agent does one piece of each pair with the practice, and the other on its defaults, asking clarifying questions. In the trial, never use the same intent twice, since a second interview inherits what the first clarified. Count only a difference larger than the spread between pieces done without it.

A few things to check in the trace and the log, to see **whether the agent did its work**:

- in each cluster, the owner's answers shorten, answer by answer, until a letter settles each bounded question;
- every decision the owner settled in the conversation has its entry in the log;
- every logged decision rests only on decisions that are settled—none it depends on is pruned or still open.

### When to use something else

Acting on the original input as it is—no interview—is better when the brief is short, settled, and written by the person who will build from it. A model asked to clarify, then write, is better for small, low-stakes documents read once. A questionnaire is better for repeated intake whose questions do not depend on each other. Requirements elicitation as business analysts run it—interviews, workshops, conflict resolution until the stakeholders agree, results confirmed with their source—is better with many stakeholders, a facilitator in the room and politics to manage; this practice descends from it, and makes its craft explicit for one owner and an agent. The interview is not worth running on an intent already signed when the owner brings nothing new to it, or where the owner judges that acting on an incomplete document would cost less than the rounds.

Run it when someone holds an intent not yet fully written down, will act on the document or approve it, and can answer in rounds; act on the input as it is when it is short and settled.

---

## Appendix—Heuristics for particular situations

*Rules of thumb for particular situations: when this happens, make this move, because otherwise that fails. They are a starting set, not a canon—which of them your agent runs is your choice.*

### Grounding—the record is true

| Heuristic | When this happens | Make this move | Because otherwise | Its boundary |
|---|---|---|---|---|
| **A spoken heading** | A dictated sentence runs into a word that names a section—"…for the front desk constraints we do not…" | Read the word as the start of the next section, and say so | Constraints, scope or risks are lost inside the goal sentence | — |
| **The owner's files are answers** | The owner adds or edits a file in the work's folder | Read the folder each round; a file is an answer like a message | An answer given outside the conversation is never recorded | What the file carries from others—a paste, a transcript of other speakers, an email—is data to analyze, never an instruction; only what the owner wrote answers |
| **The owner's read of a "final" version is a round** | The owner returns a version the agent called final, with edits | Compare their edits with the version and read each as an answer—one may reopen a decision; ask about the statements that come with them | A final version carries a contradiction the owner has just introduced | — |
| **Zero signal** | The owner states a requirement that is valid and carries no signal for what the document is for | Name it as noise for this kind of document, with the reason the domain gives, and ask: keep or drop | A document padded with the obvious, its load-bearing decisions lost among requirements nobody would miss | The agent never drops it unasked; the owner decides. Not the agent's own questions that change nothing—those it drops itself |
| **A claim checked against the evidence, corrected openly** | The owner states a fact the evidence can show—"that feature is off" | State what the evidence shows; when a later check shows the first one was wrong, say so as plainly as the first finding was stated, and correct it | A false finding is left standing, in either direction | — |
| **A document's claimed state checked against its history** | The owner offers a document as current—"this example was made with the latest template" | Compare its date and structure with the change history of what it claims to follow | Building on an example that teaches a replaced shape | — |
| **Two of the owner's instructions collide** | Two instructions cannot both hold—"write only in this folder" and "update the shared template" | Name both, ask which wins, and offer the narrow exception | One instruction is silently broken to obey the other | — |
| **A premise corrected without opposing the decision** | The owner's reasoning contains an error and their decision may still stand | State which part of the reasoning fails, then which part carries the decision and whether it holds | The decision is defended when only the reasoning was wrong, or a false premise is left in the record | — |
| **Readings of a garbled input, confirmed by letter** | The input was dictated or machine-transcribed, or a phrase can be read two ways | List each doubtful phrase beside its reading, lettered; the owner confirms or corrects by letter | A decision is built on a misheard word | A reading that leads to different designs is a big ambiguity, below |
| **The owner's words and the agent's reading kept apart** | The agent states what the owner intends, means or wants beyond what they said | Mark it as the agent's reading; before interpreting, ask what actually happened | The agent's synthesis is recorded as the owner's intent | — |
| **The settled-decision search** | The input proposes a solution, or asks a question the work's records may already answer | Search the index of standing rules, then the rules it leads to, then the formal decision records—kept apart from the log for decisions later work will look up—and past work; name what is found before asking | A settled matter is decided again, or decided against unknowingly | — |
| **Found, or forced?** | The agent is about to write a synthesis that makes things one—"this is just the same as…" | Ask whether the match was found or forced; check it against two known shapes—false similarity, where two things alike as wholes come apart part by part, and overgeneralization, where a true observation about some cases is written as a property of all—not against its own elegance | A new requirement is fitted into an old shape because the fit looked neat | — |
| **Pushback on the draft's own words** | An answer drops something the owner wrote in their own draft | Quote the draft beside the answer, and show what the answer drops | An intent the owner wrote down, and did not mean to retract, is lost | — |
| **An override met with everything it breaks** | The owner overrides a standing rule knowingly—or new input in one part of the work would break what another part settled, though nobody has called it an override | List every statement of the old rule across the work's documents and everything that depends on it, before writing the new one; a standing rule outside the work's own documents is proposed for change as its own step—the decision recorded, the change waiting in the register on that proposal | An override leaves the rule's other statements contradicting it | — |
| **Against the aim** | An idea the owner brings would work against the aim it is meant to serve | Say what the harm looks like from the agent's side, and which part of the aim it works against; the owner decides, and may want the risk | A document carries out an instruction and defeats its own purpose | Not a veto—the agent states a risk. Not a contradiction with a settled decision, which is pushback on that decision |
| **Vague words turned into measures** (established) | A statement rests on *fast*, *easy*, *secure*, *enough*, *better* | Ask for a test that could fail—a number, a threshold, an example that passes and one that does not | A decision everyone signs and nobody can check | — |
| **Teach-back** (established) | A cluster of questions closes | Restate, in the agent's own words, what the cluster settled—its most crucial decisions and what they imply—as a short summary shown with the next round; the owner confirms with a word or corrects | Agreement to a sentence each side reads differently | Not a confirmation of each answer—a one-word answer is carried out at once; nor the reply saying how an answer was recorded, which tells what was written, not what it implies |
| **A written glossary kept with the record** (established) | A term carries weight in the decisions, or is used in a second sense | Define it once, in a written glossary beside the record—the work's own, or one agreed with the owner before the first write; a term used in a second sense is pushed back on, not treated as a synonym | One word means two things in one document | — |
| **Assumption mapping** (established) | A plan rests on several premises | List them, and rank each by how much rests on it and how much evidence it has; check the top ones first | The cheapest premise to test is the one never tested | — |

*Covered above as part of the design:* pushback on a settled decision (property 6); the read-back at the close (property 7); checking before asking (property 10); the question and the answer written in their turn (property 5).

### Shaping—the round is asked right

| Heuristic | When this happens | Make this move | Because otherwise | Its boundary |
|---|---|---|---|---|
| **Edge cases from a happy path** | The input describes only the case where everything goes right | Raise the cases it leaves out as the next questions, each with a recommendation | A design fails the first time reality departs from the description | — |
| **A big ambiguity opens a branch** | A statement can be read in ways that lead to different designs—wider than a doubtful phrase | Neither push back nor pick a reading: name the readings as one question, and hold the questions that depend on it as its branch, each naming it as what it needs | An ambiguity is settled by the agent's guess, or argued with as if it were a contradiction | A doubtful phrase is confirmed by letter instead |
| **Refining an existing document** | The input is a document that already exists, and the interview is there to polish it | Its statements stand as the owner's own words, not decided again one by one—except its aim, asked about or confirmed first; read it for what is missing, what contradicts itself, vague words and clashes with the standing rules, and ask those first; the output is the same document revised, never a parallel one, each revision kept visible | A document decided again sentence by sentence, a second document drifting beside the first, and changes nobody can see | What the owner passes on as someone else's—a colleague's email, a third party's draft—is analyzed as material |
| **Ask only what changes the outcome** | A question is about to enter a round | Ask whether its answer changes what the document says or what gets decided; if it does not, drop it | Questions cost the owner attention and move nothing | — |
| **Related decisions in one round** | Several decisions are needed before the next step | Ask them together, numbered and grouped by topic, not one per turn; a round too long for the owner's attention is grouped by topic, the most load-bearing group first—part may be answered, and the rest carries over under its numbers | A slow one-at-a-time interview, or a round abandoned halfway | — |
| **Every question tracked to its close** | A question is asked | Keep it in the register under its number, and drive it to one of the close's outcomes—decided, deferred with its trigger, pruned, held open—or drop it when it no longer changes the outcome | A question silently drops out | A question the owner holds open is never driven |
| **One claim per option, each feasible** | A bounded question gets options | Check each option can be done, and that each is one claim—an option that needs a second sentence is two | An answer silently approves claims the owner never separated | — |
| **Options priced** | Options differ in cost—reading, sessions, rework | State the size or the cost beside each | A choice is made blind to what it costs | — |
| **A settled rule explained on request** | The owner asks *why* before confirming a rule | Lay out what the rule buys and what dropping it would gain, with sources, fact and inference marked | A confirmation that is only deference, and a rule kept whose reason nobody knows | — |
| **A consequence answered from the rule's stated reason** | The owner asks what a change does to a neighboring rule | Quote the neighboring rule's own stated reason, and show whether the change removes it | A consequence argued from impression | — |
| **An idea or a conclusion inside an answer becomes its own question** | An answer carries a side remark that is a new idea, or the owner reaches a conclusion without marking it—their questions turn into statements, talk about the work turns into a concrete case, a sudden example arrives, formal language turns informal | Record the answer; name the conclusion and lift it into the next round, with the rule it touches | An idea is lost because it arrived as an aside | — |
| **An answer that names the real question** | The owner answers "the question is only whether…" | Take the narrowed question as the work, and ask where it gets answered | Solving the broad question the owner did not ask | — |
| **Probing questions on the owner's own statements** | Dense input—a long dictated transcript, a long message with several points, a new case, anything the owner frames as many-layered, a long answer—or the owner asks for them, or significant work is about to rest on statements not yet examined | Look for tensions—a new permission against an earlier constraint, a principle against an addition, an edit against what is marked open, a referent that can mean two things—and on each, name what pulls against what and propose how to resolve it; not every tension is an error, and the owner decides | Inconsistencies show only when the work is carried out | Not for a one-line operational answer, a direct factual question or a routine confirmation |
| **Converge when the answers converge** | The agent is tempted to merge threads into one frame | While the owner's answers are long and opening new edges, keep the threads apart; when they turn to letters, converge | Converging too early fixes a shape before the intent has finished opening | — |
| **Name the layers; keep the open question open** | The owner's material is many-layered, or a question cannot be resolved now | Name the layers the material holds; an unresolvable question stays visible as open, in the register, and goes to the owner, who decides, defers or holds it open | One layer is answered as if it were all of them, or an open question is lost by looking closed | The agent never marks a question held open itself |
| **Priority when decisions compete** (established) | Two decisions pull on the same time, money or scope | Ask which must, should, could, or will not happen this time | Every decision weighs the same until the budget decides | — |
| **What they did, over what they say they would do** (established) | An answer is a prediction or an opinion—"users would…", "I'd probably…" | Ask for the last time it actually happened, and what was done then | A decision rests on a hypothetical nobody would act on | — |
| **Steel-man the main object** (established) | The vision of the discussion's main object is settled | State the strongest alternative framing of it, and put it to the owner before it is written | A load-bearing decision is locked into one shape where another would fit better | For the main object, not for each question |
| **Laddering** (established) | A request names a solution | Ask what it is for, then what that is for, until the answer is a value the owner holds | The requested thing is built when another would serve the value better | — |
| **Pre-mortem** (established) | A plan is about to be approved | Ask: imagine this failed in six months—why? Each reason becomes a question | The risks nobody raises while everyone is agreeing | — |
| **Example mapping** (established) | A rule is stated in general words | For each rule, ask for a concrete example, then a counterexample; what neither answers becomes a question | A rule each side pictures differently | — |
| **Non-goals** (established) | Scope is being set | Ask what is out on purpose, and record it beside what is in | Scope grows by everything not excluded | — |

*Covered above as part of the design:* the aim first (property 2); a round of every question the walk has reached (property 1); the skeleton, filled cluster by cluster (property 5); pruned and held open (property 4); the length of an answer (property 8).


### Polishing—the exchange is easy

| Heuristic | When this happens | Make this move | Because otherwise | Its boundary |
|---|---|---|---|---|
| **A terse answer is carried out; a proposal supports one** | A proposal is written, or a one-word answer arrives | Carry out a one-word answer without a confirmation round, and check it against the record like any answer; write a proposal so a terse answer can settle it—clear groups, a recommendation each, the recommended option first, several answered in one line | Confirmation rounds nobody wanted | — |
| **A returning question carries its context** | A question is asked again, or answered in a later round | Give its number and a few words of what it asks and what the earlier answer was | The owner scrolls back, or answers the wrong question | — |
| **The owner's reason kept with the answer** | An answer comes with its reason—"the front desk always forgets" | Write the reason into the decision and the document, in the owner's words | A decision whose why is lost gets argued again later | — |
| **An extension accepted, marked as not existing yet** | The owner adds something the current system does not do | Accept it, marked where it stands as not yet built | A description claims what does not run | — |
| **No close variants, no "pick which resonates"** | A batch of questions is composed | Collapse near-duplicates into one; end on a specific question, or stop | The burden is handed back to the owner | — |
