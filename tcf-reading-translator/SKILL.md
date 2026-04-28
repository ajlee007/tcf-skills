---
name: tcf-reading-translator
description: >
  Translate TCF (Test de Connaissance du Français) reading comprehension questions from French exam papers into bilingual format — French first, English below with a 5-line gap, plus a detailed answer explanation. Use this skill whenever Anjalee (or any TCF tutor/student) pastes a TCF reading comprehension question, passage, or multiple-choice item and wants it translated or formatted. Trigger for phrases like "translate this TCF question", "format this reading comprehension", "TCF paper question", "add English to this TCF", "bilingual TCF question", "translate with answer explanation", "TCF compréhension écrite", "format this for students", or any time a French reading passage + question + A/B/C/D choices appears that looks like a TCF exam item. Always use this skill — do not rely on memory alone.
---

# TCF Reading Comprehension Translator

This skill formats and translates TCF reading comprehension questions into a structured bilingual layout for students. French always comes first; English follows after a 5-line gap. Every item ends with a detailed answer explanation.

---

## Output Format (strict)

Follow this layout exactly for every question:

```
Question [N]
French Text: [Original French passage — do not alter]
Question: [Original French question — do not alter]
A. [option]
B. [option]
C. [option]
D. [option]




(5 blank lines)




English Translation: [Translated passage]
Question: [Translated question]
A. [translated option]
B. [translated option]
C. [translated option]
D. [translated option]
Answer: [Letter] - [Explanation]
```

**Rules:**
- Never alter, correct, or paraphrase the original French text or question — reproduce exactly as given.
- The 5-line gap goes **between the last French answer option (D.) and "English Translation:"** — use exactly 5 blank lines (press Enter 5 times).
- Each answer option (A, B, C, D) must be on its own separate line — never on a single line.
- The Answer explanation cites specific French phrases from the passage (with English gloss in parentheses) to justify the correct answer and briefly explain why the other options are wrong.

---

## Translation Guidelines

### Passage translation
- Translate naturally and idiomatically — aim for clarity for B1–C1 English readers.
- Preserve register: formal text stays formal, informal stays informal.
- Keep proper nouns, place names, and titles as-is.
- Do not add footnotes or clarifications inside the translation — save commentary for the Answer line.

### Answer option translation
- Translate all four options (A, B, C, D) faithfully.
- Preserve the contrast between options — the differences between them are often the whole point of the question.

### Answer explanation
Format: `Answer: [Letter] - [Explanation]`

The explanation must:
1. State why the correct answer is right — cite 1–2 key phrases from the French passage with English gloss: e.g. `"une invitation au voyage" (an invitation to travel)`
2. Briefly note why the other options are wrong or unsupported by the text (1 sentence is enough).

---

## Handling Multiple Questions

If the user pastes multiple questions (e.g. Q31, Q32, Q33), process each one in sequence using the same format. Separate questions with a single horizontal rule (`---`).

---

## Example

**Input:**
> Question 31
> La cuisine de Susan Spicer, est effectivement une invitation au voyage à travers le monde...
> Pourquoi la cuisine de Susan Spicer est-elle appréciée ?
> A. Pour ses plats simples et bon marché.  B. Pour sa gastronomie d'ici et d'ailleurs.  C. Pour ses recettes très traditionnelles.  D. Pour ses spécialités culinaires épicées.

**Output:**

```
Question 31
French Text: La cuisine de Susan Spicer, est effectivement une invitation au voyage à travers le monde. Cette quinquagénaire à la silhouette de jeune femme, règne sur la cuisine du restaurant Bayona - pas moins de 3 étoiles! - dans le Quartier français de La Nouvelle-Orléans. Née en Floride d'une mère danoise qui a été élevée en Amérique du Sud, cette femme devenue chef a pu habituer son palais, dès le plus jeune âge, aux saveurs internationales.
Question: Pourquoi la cuisine de Susan Spicer est-elle appréciée ?
A. Pour ses plats simples et bon marché.
B. Pour sa gastronomie d'ici et d'ailleurs.
C. Pour ses recettes très traditionnelles.
D. Pour ses spécialités culinaires épicées.




(5 blank lines)




English Translation: Susan Spicer's cuisine is indeed an invitation to travel around the world. This fifty-year-old woman with the figure of a young woman reigns over the kitchen of the Bayona restaurant - no less than 3 stars! - in the French Quarter of New Orleans. Born in Florida to a Danish mother who was raised in South America, this woman who became a chef was able to accustom her palate, from a very young age, to international flavors.
Question: Why is Susan Spicer's cuisine appreciated?
A. For its simple and inexpensive dishes.
B. For its gastronomy from here and elsewhere.
C. For its very traditional recipes.
D. For its spicy culinary specialties.
Answer: B - The text highlights "une invitation au voyage à travers le monde" (an invitation to travel around the world) and "saveurs internationales" (international flavors), confirming that her cuisine draws from many cultures. Options A, C, and D are not supported — the text makes no mention of low prices, traditional recipes, or spicy food.
```

---

## Edge Cases

- **No answer options given**: Still translate the passage and question; note at the end that answer options were not provided.
- **Passage already in both languages**: Format it correctly anyway — French first, 5-line gap, English second, then add the Answer explanation.
- **Question number missing**: Use "Question —" as the header.
- **Image-based questions**: Note that the image cannot be translated and ask the user to describe or paste the relevant text.
