# 🤖 The Prompt Playbook: A Recruiter's AI Assistant

Welcome to my prompt playbook! This repository contains a curated set of prompts I use as a technical recruiter to leverage Generative AI tools (like ChatGPT, Gemini, etc.) for enhanced candidate screening, interview preparation, and professional communication.

The goal is to move beyond generic, low-quality outputs by providing structured context and clear constraints, ensuring the AI acts as a reliable partner in the recruiting process.

-----

## Table of Contents

- [Syntax Guide](https://www.google.com/search?q=%23-syntax-guide)
- [Summarizing Candidate Interviews (Internal Notes)](https://github.com/harrison-tran/recruiting-prompts?tab=readme-ov-file#summarizing-candidate-interviews-internal-notes)
- [Universal Boolean Search Generation](https://github.com/harrison-tran/recruiting-prompts?tab=readme-ov-file#universal-boolean-search-generation)
- [Generating Interview Questions (Behavioral & Situational)](https://github.com/harrison-tran/recruiting-prompts?tab=readme-ov-file#generating-interview-questions-behavioral--situational)

-----

## 💡 Syntax Guide

When using the prompts below, ensure you replace all bracketed sections with the relevant information. For GitHub formatting, we'll use code blocks (` ``` `) to easily delineate the prompt text.

| Syntax | Description | Example |
| :--- | :--- | :--- |
| `[Text]` | **Required Input:** Placeholder for variable information. | `[Job Title]` |

-----

## Summarizing Candidate Interviews (Internal Notes)

This prompt helps structure raw, unstructured interview notes into a professional, concise summary suitable for sharing with a technical hiring manager. It ensures the language is tailored to a specific audience (e.g., a Data Engineer).

**Note:** For this prompt to work effectively, you must copy/paste the candidate's resume and your rough notes immediately following the prompt text.

I also included a line to remove all citations and bolding for easier pasting into an ATS. Replace Clio with your company name + description.

```
You are a technical recruiter for Clio, a legal practice management software company. You interviewed a candidate name [Candidate’s Name] for the [Job Title]. Attached is the candidate’s resume.

At the end of the prompt, I have included some rough notes taken throughout the interview. Generate a summary on the candidate’s profile using the resume attached and the rough notes provided. 

Follow these specific instructions

- Format: Maintain a point-form structure using bullet points but keep the sentences longer. Instead of using * for bullet points, use - instead. Do not use any citations or bold text.
- Headings: Organize the points under 3 headings (Professional Qualifications and Career History, Specific Project/Technical Experience, and Motivation for Looking). Professional Qualifications should have his tenure duration and more emphasis on his most recent experience. Feel free to expand on this if you feel like my rough notes are missing anything from the resume.
- Elaboration and Detail: Instead of short phrases, expand each bullet point into one or two comprehensive sentences. Combine related short notes into a single, more descriptive point. Where possible, frame the candidate's experience using the STAR method (Situation, Task, Action, Result) to add depth and context.
- Tone: Rephrase the notes to be objective and evidence-based. Replace subjective feelings (e.g., 'good vibe,' 'seems nervous') with factual observations (e.g., 'Established strong rapport,' 'Spoke quickly initially but gained confidence when discussing past projects').
- Clarity: Expand any shorthand or abbreviations into their full form (e.g., 'proj mngmt' becomes 'project management'). Correct all spelling and grammatical errors.

Rough Notes to process:


```

-----

## Universal Boolean Search Generation

This is my universal prompt to generate LinkedIn boolean searches. Feel free to remove and adjust the role requirements to your liking.

```
Act as an expert technical recruiter with deep knowledge of boolean search logic for LinkedIn.

Generate three LinkedIn boolean search strings (one broad, one specific, and one targeting specific companies) based on the detailed role requirements I provide below.

INSTRUCTIONS:
Analyze the Inputs: Carefully review all the information provided in the sections below.

Use Correct Syntax:
- Use parentheses () to group OR statements.
- Use quotation marks "" for exact, multi-word phrases (e.g., "Product Manager").
- Use AND, OR, and NOT correctly.

Generate Three Strings:
- Broad Search: A wider search focusing on core titles and a few key skills to capture a larger talent pool.
- Specific Search: A more targeted search combining seniority, specific titles, all "must-have" skills, and exclusion keywords.
- Competitor Search: A targeted search focused on finding candidates with the right title at the specified competitor companies.

--- ROLE REQUIREMENTS ---

1. Core Role Details:
- Primary Job Title: [e.g., "Product Manager"]
- Alternative Job Titles / Synonyms: [e.g., "Product Owner", "Program Manager", "Product Lead"]
- Seniority Levels to Include: [e.g., Senior, Sr., Lead, Staff, Principal]

2. Must-Have Skills & Keywords:
- Technical Skills / Tools: [e.g., SQL, Jira, Mixpanel, "A/B Testing", Python]
- Industry / Domain Keywords: [e.g., SaaS, Fintech, B2B, "Agile Methodology"]

3. Exclusion Criteria (Keywords to AVOID):
- Titles to Exclude: [e.g., Assistant, Associate, Junior, Intern, Trainee]
- Industries / Domains to Exclude: [e.g., Healthcare, Hardware]

4. Company & Location Targeting:
- Target Competitor Companies: [e.g., Google, Meta, Shopify, Slack]
- Companies to Exclude (including your own): [e.g., "My Company Inc."]
- Location: [e.g., Toronto, Canada]


```

-----

## Generating Interview Questions (Behavioral & Situational)

This prompt transforms the AI into an expert Hiring Manager, creating highly relevant, probing questions based on a candidate's specific resume achievements. It moves beyond generic questions to encourage **STAR method** (Situation, Task, Action, Result) answers.

This is best used when you're new to a specific role and trying to learn on the go! Adding the job description to the prompt will elevate this even further.

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
