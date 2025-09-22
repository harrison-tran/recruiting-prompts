# 🤖 The Prompt Playbook: A Recruiter's AI Assistant

Welcome to my prompt playbook! This repository contains a curated set of prompts I use as a technical recruiter to leverage Generative AI tools (like ChatGPT, Gemini, etc.) for enhanced candidate screening, interview preparation, and professional communication.

The goal is to move beyond generic, low-quality outputs by providing structured context and clear constraints, ensuring the AI acts as a reliable partner in the recruiting process.

-----

## Table of Contents

- [Syntax Guide](https://www.google.com/search?q=%23-syntax-guide)
- [Generating Interview Questions (Behavioral & Situational)](https://www.google.com/search?q=%232-generating-interview-questions-behavioral--situational)
- [Summarizing Candidate Interviews (Internal Notes)](https://www.google.com/search?q=%233-summarizing-candidate-interviews-internal-notes)

-----

## 💡 Syntax Guide

When using the prompts below, ensure you replace all bracketed sections with the relevant information. For GitHub formatting, we'll use code blocks (` ``` `) to easily delineate the prompt text.

| Syntax | Description | Example |
| :--- | :--- | :--- |
| `[Text]` | **Required Input:** Placeholder for variable information. | `[Job Title]` |

-----

## Generating Interview Questions (Behavioral & Situational)

This prompt transforms the AI into an expert Hiring Manager, creating highly relevant, probing questions based on a candidate's specific resume achievements. It moves beyond generic questions to encourage **STAR method** (Situation, Task, Action, Result) answers.

```
Act as the Hiring Manager for the [Department Name] team. You are an expert in [Field, e.g., 'Product Management'] and are looking to deeply understand a candidate's thought process and past achievements.

Generate a list of behavioral interview questions based on specific points from the candidate's resume.

Context
- Job Title we are hiring for: [Job Title]
- Candidate's Name: [Candidate Name]
- Key Resume Achievement #1: [Copy/paste a specific achievement from their resume, e.g., "Grew organic traffic by 150% in 12 months"].
- Key Resume Achievement #2: [Copy/paste another achievement, e.g., "Managed a cross-functional team of 8 to launch the new mobile app"].
- Core competency we need to assess: [Mention a key skill, e.g., 'Data-Driven Decision Making' or 'Leadership'].

Questions should be open-ended and behavioral, like this example: "Your resume says you 'Grew organic traffic by 150%'. Can you walk me through the specific strategies you implemented to achieve that? What was your personal contribution?"

Organize the questions into sections based on the resume achievements and competencies provided.
- Questions about [Key Resume Achievement #1]
- Questions about [Key Resume Achievement #2]
- Questions assessing [Core Competency]

The tone of the questions should be probing, insightful, and professional. They should be designed to encourage storytelling and detailed examples (using the STAR method), not simple 'yes/no' answers.
```

-----

## Summarizing Candidate Interviews (Internal Notes)

This prompt helps structure raw, unstructured interview notes into a professional, concise summary suitable for sharing with a technical hiring manager. It ensures the language is tailored to a specific audience (e.g., a Data Engineer).

**Note:** For this prompt to work effectively, you must copy/paste the candidate's resume and your rough notes immediately following the prompt text.

```
You are a technical recruiter for Clio, a legal practice management software company. You interviewed a candidate name [Candidate’s Name] for the [Job Title]. Attached is the candidate’s resume.

Below I have included some rough notes taken throughout the interview. Generate a summary on the candidate’s profile using the resume attached and the rough notes provided. Organize these notes into three headings (Professional Qualifications, Project/Technical Experience, and Motivation for Looking). Keep the language professional as if you were sending this to the hiring manager, who is a data engineer himself.
```
