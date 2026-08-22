# AI-Assisted ICU Quality Review Workbench

This repository contains the static project website for Group 6.

## Project Name

AI-Assisted ICU Quality Review Workbench

## Website

The website is available through GitHub Pages:

https://mohamd-mh.github.io/2026_group6_AI_Assisted_ICU_Quality_Review_System/

## Software Repository

The runnable software source code is available here:

https://github.com/domainenguoh/icu-risk-workflow-final

## Repository Contents

- `index.html` — main website entry page
- `assets/` — website CSS, images, and screenshots
- `pages/` — project pages, user manual, evaluation, related work, and documentation
- `downloads/` — downloadable project materials, including the software ZIP, report, presentation, papers, and related files

## Notes

This project is an academic prototype. It supports retrospective ICU quality-review prioritization and documentation using processed de-identified MIMIC-III data. It is not a clinical diagnosis system, treatment system, live ICU monitor, or official medical scoring tool.

## Coordinator Role, Output, and Real-Time Scope

The coordinator is the human link between the processed ICU data, the AI review signals, and the review team. The system does not expect the review team to read raw CSV files, model probabilities, scattered vital signs, or unorganized case details. Instead, the coordinator uses the workbench to turn all of that information into a clear review package. The coordinator starts by opening the Dashboard and selecting the next case that should be reviewed. Then they open the Review Ticket, check the AI risk level, SIRS-style screening result, data quality, similar cases, anomaly signals, uncertainty level, and explanation signals. If more context is needed, they open the Case Safety Profile to understand why the case was flagged. After that, they add coordinator notes, complete the checklist, generate a Prepared Review Summary, update the status, and send the case forward as Ready for Quality Team Review.

The coordinator’s final output is not a diagnosis and not a treatment decision. The final output is a structured Review Ticket that contains the case priority, AI risk explanation, SIRS screening result, important vitals and labs, uncertainty/anomaly context, coordinator notes, checklist status, prepared summary, review outcome, status history, and audit trail. This helps the review team because they receive an organized case summary instead of starting from raw data or disconnected AI outputs. The coordinator saves them time, makes the review process more consistent, explains why each case was prioritized, and keeps a traceable record of what was reviewed and what action was taken.

The system is also not a real-time monitoring system. It does not connect to live ICU machines, does not receive live patient data, does not send emergency alerts, and does not tell doctors what treatment to give. In this project, the data comes from historical, de-identified ICU stays from MIMIC-III, meaning the cases already happened in the past and no real patient identity is shown. The purpose is retrospective quality review: the coordinator reviews past ICU stays, understands the AI and rule-based signals, documents the case, prepares a summary, and passes it to the review team. A future version could support live integration, but that would require security, privacy approval, clinical validation, and real-world deployment. Our prototype focuses on the engineering workflow: data processing, AI signals, explanation, documentation, handoff, status tracking, and audit history.

## How to Run the Software

Download `Software_System.zip` from the website Downloads page, extract it, open a terminal inside the extracted `Software_System` folder, and run:

```bash
python app.py
