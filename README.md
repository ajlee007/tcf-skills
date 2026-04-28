# 🇫🇷 TCF Skills — Claude AI Skill Files for French Exam Preparation

A collection of Claude skill files (`.md`) for teaching and preparing students for the **TCF (Test de Connaissance du Français)** and **TEF Canada** exams. Built for French tutors, language educators, and self-study learners.

These skills are designed to be used with [Claude](https://claude.ai) and [Claude Code](https://claude.ai/code) as part of an AI-powered French tutoring workflow.

---

## 📁 Skills in this repo

| Skill file | What it does | Best for |
|---|---|---|
| `tcf-ai-tutor/SKILL.md` | Full TCF exam prep tutor — grammar, vocab, speaking, reading, writing across A1–C2 | Tutors building complete lesson materials |
| `tcf-speaking-roleplay/SKILL.md` | Live interactive TCF Canada Expression Orale simulator — Claude plays the examiner | Students practising oral tasks in real time |
| `tcf-b1b2-answer-generator/SKILL.md` | Generates B1–B2 model answers for all three TCF/TEF Canada Expression Écrite tasks | Intermediate learners and immigration exam candidates |
| `tcf-reading-translator/SKILL.md` | Translates TCF reading comprehension questions into bilingual French/English format | Tutors creating student-facing worksheets |

---

## 🎯 Who this is for

- **French tutors** teaching TCF/TEF Canada exam candidates
- **Students** preparing for TCF, TEF Canada, DELF, or DALF
- **Immigration applicants** targeting B1–B2 for NCLC requirements
- **AI educators** building Claude-powered language tutoring workflows

---

## 🚀 How to use these skills

### Option 1 — With Claude.ai (Projects)
1. Open [Claude.ai](https://claude.ai) and create a new Project
2. Upload the relevant `SKILL.md` file as a Project document
3. Start a conversation — Claude will follow the skill instructions automatically

### Option 2 — With Claude Code
1. Clone this repo into your project folder:
   ```bash
   git clone https://github.com/ajlee007/tcf-skills.git
   ```
2. Reference the skill file path in your `CLAUDE.md` or pass it directly in your prompt
3. Claude Code will read and apply the skill during your session

### Option 3 — Copy & paste
Open any `SKILL.md`, copy the contents, and paste it as a system prompt in Claude or any Claude-compatible interface.

---

## 📋 Skill summaries

### `tcf-ai-tutor`
A comprehensive TCF exam preparation tutor covering all five skill domains. Generates structured, markdown-only study materials with English translations, phonetic guides, answer keys, and word banks. Supports A1–C2 levels. Applies Canadian French rules when requested.

**Triggers:** `"TCF practice"`, `"French grammar exercise"`, `"TCF speaking prompt"`, `"reading comprehension"`, `"TCF writing"`

---

### `tcf-speaking-roleplay`
An interactive TCF Canada Expression Orale simulator. Claude plays the examiner and conducts a live back-and-forth role-play in French. Covers 10 topic themes (housing, work, travel, health, etc.) and simulates both Tâche 2 (interactive) and Tâche 3 (opinion/debate).

**Triggers:** `"let's do a role play"`, `"TCF speaking practice"`, `"simulate the oral exam"`, `"practice Tâche 2"`

---

### `tcf-b1b2-answer-generator`
Generates realistic, examiner-ready model answers at B1 and B2 level for all three TCF/TEF Canada Expression Écrite tasks. Designed for intermediate learners who need honest, achievable targets — not polished C1 prose they can't reproduce under exam conditions.

**Triggers:** `"give me a B1 answer"`, `"B2 response for tâche 1"`, `"intermediate level TCF answer"`

---

### `tcf-reading-translator`
Formats and translates TCF reading comprehension questions into a strict bilingual layout — French first, English after a 5-line gap, with a detailed answer explanation citing the original French text. Designed for tutors creating print-ready student worksheets.

**Triggers:** `"translate this TCF question"`, `"bilingual TCF question"`, `"format this for students"`

---

## 🗂️ Repo structure

```
tcf-skills/
├── README.md
├── tcf-ai-tutor/
│   └── SKILL.md
├── tcf-speaking-roleplay/
│   ├── SKILL.md
│   └── references/
│       └── prompt-bank.md
├── tcf-b1b2-answer-generator/
│   └── SKILL.md
└── tcf-reading-translator/
    └── SKILL.md
```

---

## 👩‍💻 About

Built by [Anjalee](https://github.com/ajlee007) — AI educator, automation specialist, and French language tutor based in Colombo, Sri Lanka. These skills are part of a broader AI-powered tutoring workflow serving TCF/TEF Canada exam candidates across Sri Lanka, Australia, and New Zealand.

Follow along on [LinkedIn](https://www.linkedin.com/in/anjaleeperera/) for more AI workflow and education content.

---

## 📄 License

MIT — free to use, adapt, and share with attribution.
