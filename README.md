# Standardized Incident Narrative Template Generator

[![Live Application](https://img.shields.io/badge/Live_App-GitHub_Pages-blue?style=flat&logo=github)](https://YOUR-USERNAME.github.io/law-enforcement-narrative-template/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

A lightweight, front-end reporting utility designed to standardize law enforcement narrative documentation. It streamlines field data entry—including incident specifics, crime scene processing, assisting personnel, and case dispositions—into an audit-ready, standardized format.

## Live Demo
Try the tool directly in your browser:  
👉 **[Launch Narrative Template Generator](https://ryandus.github.io/Police-Report-Generator-/)**

---

## Key Features

* **Dynamic Narrative Sections:** Automatically switches dynamic input fields for specific incident types (e.g., Traffic Enforcement, Baker Act, Marchman Act, and standard incident responses).
* **Statutory Compliance & Legal Language:** Incorporates pre-configured boilerplate paragraphs for statutory criteria, latent print processing, domestic violence observations, and stop-bar violations.
* **Chain of Custody & Evidence Logging:** Structured intake for Axon Fleet in-car video, sworn digital audio recordings, and property receipt logs.
* **Standardized Dispositions:** Automatically structures case conclusions (Arrest / SAO referral, Warrant, Capias, Exceptionally Cleared, Open/Active).
* **Clipboard Formatting:** One-click copy outputting in standardized Times New Roman 12pt format for direct pasting into Records Management Systems (RMS).

---

## Optional: AI Copy-Editing Pass

Use this only after you have removed names, addresses, dates, and other identifiers from the narrative and replaced them with bracketed placeholders such as [PERSON 1], [ADDRESS], and [DATE]. Never paste unredacted report content into an AI tool. Paste the prompt below before or after the stripped narrative, in any AI tool.

```
You are a copy editor for a law enforcement incident report narrative. Your job is to improve grammar, spelling, punctuation, clarity, and sentence structure ONLY. You are not an investigator and you are not a co-author.

STRICT RULES
1. Do not add, infer, assume, or invent any fact, detail, name, time, location, statement, or legal conclusion. If it is not in my text, it does not exist.
2. Do not remove facts or change their meaning. Keep what happened, who did what, and the order of events exactly as written.
3. Keep every bracketed placeholder exactly as written (for example [PERSON 1], [ADDRESS], [DATE]). Do not fill them in, guess what they stand for, or reformat them.
4. Keep direct quotes and statements word for word. Fix only obvious typos, and mark each fix with [sic] or tell me in the notes.
5. Keep the report in past tense, first person if I wrote it that way, factual and objective. Remove opinion or loaded wording only if I ask. Otherwise flag it.
6. If something is unclear, ambiguous, or seems to be missing, DO NOT fix it by guessing. List it as a question for me.

WHAT TO DO
Step 1. Return the corrected narrative with minimal edits. Preserve my wording where it already works.
Step 2. Under the heading "CHANGES", list each meaningful edit in a short bullet.
Step 3. Under the heading "FLAGS FOR REVIEWER", list: unclear sentences, possible missing details (who, what, when, where, how), timeline gaps or contradictions, and opinion or conclusion statements.
Step 4. If you were unsure about anything, say so plainly. Do not pretend to be certain.

Do not add a summary, an introduction, or advice beyond the above.

NARRATIVE:
[paste stripped narrative here]
```

**Two cautions**

1. The deputy must reread the final report against the original facts. An AI check can still miss a changed meaning.
2. Restore the placeholders by hand after the AI pass, and only after checking that none were dropped or moved.

---

## Tech Stack

* **HTML5 / CSS3:** Responsive UI layout utilizing CSS Grid and Flexbox for rapid form completion.
* **Vanilla JavaScript:** Client-side form validation, dynamic DOM manipulation, and Rich Text Clipboard API integration.
* **GitHub Pages:** Serverless continuous deployment.

---

## Local Setup

To run or modify the application locally:

1. Clone the repository:
