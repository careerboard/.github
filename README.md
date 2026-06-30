# CareerBoard

**CareerBoard is an AI-powered job search workflow system for people who want to apply with strategy, not spam.**

It helps candidates collect vacancies, evaluate fit, tailor resumes and cover letters, prepare for interviews, and keep the whole job search organized in one place.

The project started as a personal resume tailoring tool and grew into a full workflow system around modern AI-assisted hiring.

## What CareerBoard does

CareerBoard is built around a simple idea:

> A job application is not just a resume.  
> It is a workflow.

For each vacancy, CareerBoard can help with:

- evaluating whether the role is a good fit
- tailoring a resume to the specific job description
- generating a matching cover letter
- tracking application status on a board
- preparing for interviews using the exact vacancy and submitted resume
- storing generated files and artifacts
- syncing PDFs into a local folder structure
- integrating with external tools through API and agent-friendly interfaces

## Core features

### AI vacancy evaluation

CareerBoard can analyze a job page or job description and compare it with the candidate profile.

It helps answer questions like:

- Is this role actually relevant?
- Which skills match?
- What are the risks?
- Is it worth applying?

### Resume and cover letter tailoring

CareerBoard generates structured resumes and cover letters based on:

- the vacancy description
- the candidate profile
- selected model settings
- target language
- resume structure rules
- real experience only, without invented skills or fake seniority

The goal is not to create a "better fictional candidate".  
The goal is to present the real candidate in the most relevant way for each role.

### Job search board

Every vacancy lives inside a board with its own status, notes, generated files, interview materials, and history.

This makes the job search easier to manage than a random folder full of PDFs named `resume-final-final-23.pdf`.

### Interview preparation

CareerBoard can use the vacancy, resume, company context, and candidate profile to help prepare for interviews.

Instead of generic interview tips, the system works with the exact opportunity.

### Background AI operations

Long-running AI tasks are executed asynchronously through background workers.

This makes expensive operations more reliable:

- browser tab can be closed
- tasks can be retried
- task status is stored
- generated artifacts are persisted
- billing can be settled safely

### PDF generation

Generated resumes and cover letters are exported as stable PDFs using a controlled server-side rendering pipeline.

The preview and final PDF are based on the same structured data, which helps keep the result consistent across devices.

### Private file storage

CareerBoard treats personal documents as private by default.

Generated PDFs, uploaded photos, attachments, and other files are stored in private object storage and accessed through short-lived signed URLs.

### Local file autosync

CareerBoard can sync generated PDFs into a local folder structure using the browser File System Access API.

This gives users clean local folders for companies, vacancies, resumes, and cover letters without manually downloading and renaming files every time.

### Browser extension

The CareerBoard browser extension makes it possible to evaluate job pages directly from the browser.

Open a job page, run evaluation, check fit, and send good vacancies into the workflow.

Chrome Web Store:

https://chromewebstore.google.com/detail/bfpdocnfigcgaeceodldnlpbpgbkilpo

### Public API

CareerBoard exposes a public API for integrations, tools, and external clients.

API documentation:

https://api.careerboard.app/public-api-docs

Node.js API client:

https://github.com/careerboard/api-client


## Why this exists

Modern hiring is increasingly filtered by ATS systems, AI screeners, automated workflows, and high competition.

Sending the same generic resume everywhere is usually not enough.

At the same time, spamming hundreds of applications is not a great strategy either.

CareerBoard tries to help candidates apply more intentionally:

- understand the fit before applying
- tailor applications honestly
- keep the process organized
- prepare better for interviews
- reduce repetitive manual work

## Project status

CareerBoard is an actively developed product.

Some parts are production-facing, some are experimental, and some repositories in this organization may contain supporting tools, API clients, documentation, integrations, or prototypes.

## Links

Website:

https://careerboard.app

App:

https://my.careerboard.app

Public API docs:

https://api.careerboard.app/public-api-docs

Node.js API client:

https://github.com/careerboard/api-client

Chrome extension:

https://chromewebstore.google.com/detail/bfpdocnfigcgaeceodldnlpbpgbkilpo

## About

CareerBoard was created by Ilia Rychagov as a personal job search system and later grew into a broader AI workflow product for structured, intentional job applications.
