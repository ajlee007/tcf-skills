---
name: tcf-b1b2-answer-generator
description: >
  Generates high-scoring B1–B2 model answers for TCF/TEF Canada Expression Écrite tasks (Tâche 1, 2, and 3).
  Use this skill whenever a student at B1 or B2 level asks for a sample answer, model response, corrected example,
  or writing help for any TCF or TEF Canada written expression task at beginner-intermediate level.
  Also use when a student says their French is "not very advanced", "intermediate", "basic but improving",
  or when they want to understand what a B1 or B2 answer looks like before aiming for C1.
  Triggers include: "give me a B1 answer", "write a B1-B2 sample for TCF", "what does a B1 response look like",
  "intermediate level TCF answer", "model answer for B1", "TCF B1 writing example", "B2 response for tâche 1",
  "beginner TCF written answer", "help me write for TCF at B1 level", or any request for TCF/TEF writing
  specifically at B1 or B2 level. Always use this skill — do not rely on memory alone.
---

# TCF/TEF Canada — Expression Écrite Answer Generator (B1–B2)

Generate clear, accurate, examiner-ready model answers at **B1 and B2 level** for all three written expression tasks of the TCF/TEF Canada exam. Designed for intermediate learners who need realistic targets — not overwhelming C1 sophistication.

---

## Why B1–B2 Matters

- **B1 (NCLC 5–6):** Minimum threshold for many immigration streams; answers must be clear and functional
- **B2 (NCLC 7):** The most common immigration target; strong but not yet academic
- This skill targets students who are **building confidence** and need to see what a real B1 or B2 answer looks like — with simpler vocabulary, shorter sentences, and honest grammar — not polished C1 prose they can't reproduce under exam conditions

---

## The Three Tasks — Rules & Structure

### Tâche 1 — Short Message (60–120 words, ~10 min)
**Purpose:** Communicate clearly to a specific recipient.
**Register:** Informal (tu) for friends/family; formal (vous) for boss/strangers.

**Required structure:**
1. **Subject line** (if email format)
2. **Salutation** — appropriate to the relationship
3. **Opening purpose** — why you are writing (1–2 sentences)
4. **Details** — Qui? Quoi? Quand? Où? Avec qui?
5. **Concrete ask or expectation**
6. **Closing formula** — À bientôt / Cordialement / Amicalement

### Tâche 2 — Article / Blog / Letter (120–150 words, ~20 min)
**Purpose:** Describe an experience or share an opinion with a title.

**Required structure:**
1. **Title** — simple and relevant
2. **Introduction** — what the topic is (1 sentence)
3. **Personal experience or description** — concrete, specific
4. **Recommendation or opinion** — what you think or suggest

### Tâche 3 — Argumentative Synthesis (120–180 words, ~30 min)

**Sub-parts:**
- **Part A (40–60 words):** Neutral summary of TWO documents
- **Part B (80–120 words):** Your personal opinion with at least 2 reasons

**Required structure:**
1. **Title**
2. **Synthesis of Doc A + Doc B** — balanced, no opinion
3. **Your position** — clearly stated with examples

---

## B1 vs B2 — What Changes

| Feature | B1 | B2 |
|---|---|---|
| **Sentences** | Short, clear, mostly simple | Mix of simple + compound; some subordinate clauses |
| **Vocabulary** | Common, everyday words | Some varied synonyms; avoids repetition |
| **Connectors** | mais, et, donc, parce que, aussi | cependant, en revanche, par conséquent, de plus |
| **Grammar** | Présent, passé composé, futur simple | + Imparfait, conditionnel présent, relative clauses |
| **Errors** | Minor errors allowed (agreement, accent) | Very few errors; structures used mostly correctly |
| **Register** | Appropriate but may be slightly stiff | Naturally appropriate to context |
| **Task completion** | All parts addressed | All parts addressed with relevant detail |

**B1 is NOT:**
- Slang or texting language
- Incomplete answers
- Ignoring part of the prompt

**B2 is NOT:**
- Academic or literary language
- Subjunctive used everywhere
- Idiomatic turns that only advanced speakers use naturally

---

## Output Format (follow exactly)

**CRITICAL — FILE OUTPUT:** Every response MUST be saved as a `.md` file and presented to the student for download. Use the `create_file` tool to write to `/mnt/user-data/outputs/[task-slug]-b1b2.md` (e.g. `tache2-vacances-b1b2.md`), then use `present_files` to share it.

For EVERY prompt the student gives, produce the following output IN THIS EXACT ORDER:

---

### ORIGINAL PROMPT

*[The original French prompt, copied verbatim]*

**English:** *[Full English translation of the prompt]*

---

### ANSWER SKELETON

Plan the answer paragraph by paragraph BEFORE writing it. This teaches students how to think before writing under exam pressure.

**Format:**
- **Para 1 — [Structural label] :** [What to write here] *[2–3 simple vocabulary items or phrases to use]*
- **Para 2 — [Structural label] :** [What to write here] *[2–3 vocabulary items]*
- ...

For Tâche 1: Subject line / Salutation / Opening purpose / Details / Ask / Closing
For Tâche 2: Title / Introduction / Experience & details / Recommendation
For Tâche 3: Title / Part A (Doc A summary + Doc B summary) / Part B (position + reason 1 + reason 2 + closing)

---

### MODEL ANSWER — [Tâche X] — Level [B1 / B2]

*[The full model answer in French — natural, achievable, realistic for the stated level]*

**Nombre de mots : [X]**

---

### ENGLISH TRANSLATION

*[Full natural English translation of the answer]*

---

### VOCABULARY FOCUS

| French Expression | English Meaning | Level | Why It Helps |
|---|---|---|---|
| [expression] | [meaning] | B1 / B2 | [why a student should learn this: common, versatile, shows range] |

Aim for **8–10 entries**. Focus on: useful connectors, everyday-but-varied vocabulary, functional phrases, register-appropriate formulas. Keep it achievable — these should be words and phrases a B1/B2 student CAN use in an exam.

---

### ANSWER STRUCTURE BREAKDOWN

Map the answer to its required components. Each line names the structural element and says what was written.

- [Structural element] — [What was done]
- ...

---

### KEY PHRASES TO REUSE

| Phrase | Use it when... |
|---|---|
| [phrase] | [situation where this phrase works across multiple prompts] |

6–8 entries. Focus on transferable sentence starters, opinion-launching phrases, transition formulas, and closing expressions that a B1/B2 student can memorise and reuse.

---

### WHY THIS IS A B1/B2 ANSWER

An honest, encouraging examiner-style explanation of WHY this answer sits at B1 or B2 — and what a student would need to change to reach the next level.

**Task Completion & Communication** — [Were all parts of the prompt addressed? Was the message clear and functional?]

**Vocabulary (Richesse lexicale)** — [What vocabulary choices signal B1 or B2? What's appropriately simple? What shows range without being overreaching?]

**Grammar & Syntax (Correction grammaticale)** — [What structures were used? Were they used correctly? What would push this answer up to B2 or C1?]

**Coherence & Cohesion (Cohérence et cohésion)** — [How were ideas linked? Were connectors used correctly and naturally?]

**Register & Adaptation (Adéquation au contexte)** — [Was the register appropriate? Was tu/vous correct? Were salutation and closing formulas natural?]

**Overall Level: B1 / B2** — [One or two honest sentences. What lifts it above B1? What would need to change to reach C1?]

---

## B1–B2 Connector Bank

**Basic connectors (B1):**
- et, mais, donc, parce que, alors, aussi, ensuite, d'abord, enfin
- Je pense que / Je crois que / À mon avis / Selon moi
- Par exemple / Comme / C'est-à-dire

**More varied connectors (B2):**
- De plus / En outre / Par ailleurs / Cependant / En revanche / Néanmoins
- C'est pourquoi / C'est la raison pour laquelle / Grâce à / Malgré
- Il me semble que / J'estime que / À mon sens

**Tâche 3 synthesis openers (B1–B2):**
- "Ces deux documents parlent de [sujet]."
- "Le premier document montre que... tandis que le deuxième explique que..."
- "D'un côté... de l'autre..."

**Tâche 3 opinion openers (B1–B2):**
- "À mon avis, [position]."
- "Je pense que [position] parce que [raison]."
- "Pour ma part, il me semble que..."

---

## Useful Grammar Structures by Level

### B1 — Use these correctly
- Passé composé: J'ai décidé de... / Nous sommes allés...
- Futur simple: Je vais / Il sera possible de...
- Conditionnel (wish/suggestion): Je voudrais / Ce serait bien si...
- Relative clauses (simple): C'est un endroit qui est très calme.

### B2 — Also use these
- Imparfait for background/description: Quand j'étais enfant, je...
- Conditionnel in argument: Il serait préférable de...
- Gérondif: En travaillant régulièrement, on peut...
- Nominalisation (simple): La pratique du sport / Le développement de...

---

## Quality Checklist (verify before producing output)

- [ ] Word count within required range
- [ ] All parts of the prompt addressed
- [ ] Register (tu/vous) matches the prompt's recipient
- [ ] No slang or text-message language
- [ ] Vocabulary is varied but not artificially elevated beyond the level
- [ ] Connectors are correctly used (not overloaded)
- [ ] Title included for Tâche 2 and Tâche 3
- [ ] Both document viewpoints represented neutrally in Tâche 3 Part A
- [ ] Clear personal opinion with at least 2 reasons in Tâche 3 Part B
- [ ] Vocab table has 8–10 entries with honest level labels
- [ ] "Why this is B1/B2" section is specific and actionable (not generic praise)

---

## Sample — Tâche 1 at B1 (to calibrate tone)

**Prompt:** Vous avez manqué la réunion de travail de votre collègue. Envoyez-lui un message pour vous excuser et lui demander les informations importantes.

**Model Answer (B1):**

**Objet : La réunion d'hier**

Bonjour Marc,

Je t'écris pour m'excuser. Hier, je n'ai pas pu assister à la réunion parce que j'étais malade. Je suis vraiment désolé(e).

Est-ce que tu peux me donner les informations importantes ? J'aimerais aussi avoir les décisions prises pendant la réunion. Si tu as des documents, tu peux me les envoyer par email.

Merci beaucoup pour ton aide. Je te promets d'être présent(e) à la prochaine réunion.

À bientôt,
[Prénom]

*(75 mots)*

---

## Sample — Tâche 3 at B2 (to calibrate tone)

**Prompt:** Deux documents sur le télétravail. Rédigez une synthèse des deux points de vue, puis donnez votre opinion.

**Model Answer (B2):**

**Le télétravail : avantage ou inconvénient ?**

Ces deux documents présentent des opinions différentes sur le télétravail. Le premier document montre que travailler à domicile permet de mieux organiser sa journée et d'économiser du temps. En revanche, le deuxième document explique que certains employés se sentent isolés et ont du mal à séparer leur vie professionnelle de leur vie personnelle.

À mon avis, le télétravail peut être positif si on le pratique de façon équilibrée. D'abord, il permet d'éviter les transports fatigants et de travailler dans un environnement calme. De plus, on peut mieux gérer son temps. Cependant, il est important de garder du contact avec ses collègues pour ne pas se sentir seul. Pour ma part, je préférerais travailler à domicile deux ou trois jours par semaine.

*(148 mots)*
