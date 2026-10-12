[AI-Ready Accountant](#top)

[**01**Basics](#basics) [**02**Use cases](#usecases) [**03**Tools](#tools) [**04**Prompting](#prompting) [**05**Automation](#automation) [**06**Safety](#safety) [**07**8-week plan](#plan) [**08**Library](#library)

A field manual for finance professionals · UAE & Middle East

# Close the books faster with *AI as your junior*

Written for an internal accountant at an IT services and consulting company, with no technical background assumed. Eight modules take you from "what is AI?" to running your own invoice, reconciliation and reporting automations, using tools your company most likely already pays for.

**How to use this site:** read modules 01–04 in your first week (about 3 hours total). Then follow the 8-week plan in module 07, doing one automation recipe from module 05 every two weeks. Each module ends with something to try at your desk the same day.

JV-2026-10 · Time reallocationhrs / month

| Dr Analysis & business partnering | 24.0 |
| --- | --- |
| Cr Manual invoice keying | (10.0) |
| Cr Reconciliation matching | (8.0) |
| Cr Variance commentary drafting | (6.0) |
| Net change in effort | 0.0 |

The goal is a reclassification, not a write-off. AI takes the keying and matching; you keep the judgement. Figures are illustrative.

01

Module 01 · 45 minutes

## AI in plain language

You do not need to know how an engine works to drive a car. You do need to know what the pedals do, how far the tank goes, and when to brake. This module is the pedals.

**The one analogy to remember:** modern AI is a brilliant new intern who has read millions of books, contracts and accounting standards, types at lightning speed, works 24/7, but has never been inside your company, does not know your numbers, and will sometimes answer confidently when it should have said "I don't know". You would never let a new intern post a journal without review. Treat AI the same way.

### The family tree, from broad to specific

Artificial Intelligence (AI)

#### Computers doing tasks that normally need human thinking

The umbrella term. Includes everything from spam filters to ChatGPT.

"Finance" as a word: it covers AP, tax, treasury and FP&A, each doing very different work.

Machine Learning (ML)

#### Learning rules from examples instead of being programmed

Nobody writes "if vendor = du then GL 6120". The system studies 10,000 past invoices and works out the pattern itself.

A junior who learns GL coding by watching how the team coded last year's invoices, rather than reading a manual.

Generative AI / LLM

#### AI that writes new text, tables, code or images

A Large Language Model (ChatGPT, Microsoft Copilot, Claude, Gemini) predicts the next most likely word, over and over, after reading a huge share of the internet's text.

Your phone's autocomplete, scaled up a million times, so it can finish an entire memo instead of one word.

AI Agent

#### AI that takes actions, not just answers

An agent can open files, run a reconciliation, send a reminder email or update a spreadsheet, following a goal you set.

The difference between an intern who tells you which invoices are overdue and one who also drafts and queues the chaser emails for your approval.

### Seven terms you will hear in every meeting

| Term | What it means | Accounting analogy |
| --- | --- | --- |
| Prompt | The instruction you type to the AI. | The briefing email you send a junior. Vague brief, vague work. |
| Hallucination | AI states something false as if it were true (a made-up IFRS paragraph number, a wrong total). | A plausible-looking figure plugged in to make a schedule balance. Always tick and bash. |
| Context window | How much text the AI can "see" at once in a conversation. | The size of the intern's desk. Papers that fall off the desk are forgotten. |
| Grounding / RAG | Making the AI answer from your own documents rather than from memory. | An open-book exam versus a closed-book one. Open-book answers are far more reliable. |
| Token | A chunk of text (roughly ¾ of a word) that AI tools count and charge by. | The billable unit, like a consultant's hour. |
| RPA | Robotic Process Automation: software that repeats exact clicks and keystrokes. | A vending machine: perfect for identical, rule-based steps; useless when the invoice layout changes. |
| Human-in-the-loop | A person reviews before AI output is used or posted. | Maker-checker control. AI is the maker; you stay the checker. |

### What AI is good at, and where it fails

#### Strong (use it freely, still review)

- Summarising long contracts, SOWs, audit letters and policies
- Drafting emails, variance commentary, memos, board-pack narrative
- Explaining or writing Excel formulas, Power Query steps and macros
- Reading invoices, receipts and PDFs and pulling out fields
- Translating Arabic ↔ English correspondence
- Spotting unusual items in a list (duplicates, outliers, odd vendors)

#### Weak (never trust without checking)

- Arithmetic done "in its head" inside a chat. Let Excel do the maths.
- Citing exact tax law articles, IFRS paragraphs or FTA rulings
- Anything after its training date unless it searches the web
- Your company's specific policies, unless you give them the document
- Final judgement calls: provisions, revenue cut-off, impairment

**Watch first (8 minutes):** [Large Language Models explained briefly](https://www.youtube.com/watch?v=LPZh9BOjkQs) by 3Blue1Brown, made for the Computer History Museum. It is the clearest non-technical explanation available. **Try today:** open Microsoft Copilot (or your company's approved AI tool) and ask, "Explain IFRS 15 five-step model to me as if I were a first-year trainee, using an IT consulting project as the example." Use Microsoft 365 Copilot, your company's approved tool. Then check its answer against what you know. That is the habit this whole course builds.

02

Module 02 · 40 minutes

## Where AI fits in your job

An IT services company in the Middle East has a very particular finance profile: project-based revenue, offshore delivery centres charging back costs, six Gulf currencies, VAT at different rates, a new corporate tax and a national e-invoicing mandate arriving in 2027. Here is where AI helps in each.

| Area | The pain today | What AI does | Tool | Effort |
| --- | --- | --- | --- | --- |
| Project revenue & unbilled (IFRS 15) | Reading SOWs to find milestones, change requests and acceptance clauses for fixed-price and T&M projects. | Summarises each contract into a one-page table: billing triggers, payment terms, retention, penalties, performance obligations. | Copilot / Claude / ChatGPT (approved) | Easy |
| Timesheet-to-invoice leakage | Billable hours logged but never invoiced, spotted months later. | Compares timesheet export vs billing register, flags gaps by project and consultant. | Copilot in Excel, Power Query | Medium |
| Intercompany recharges | Offshore delivery centres (e.g. India) cross-charge costs; mismatches between entities at month-end. | Matches both sides of intercompany balances, explains differences (FX, timing, missing invoice). | Copilot Financial Reconciliation agent | Medium |
| Multi-currency GCC consolidation | AED, SAR, QAR, KWD, OMR, BHD trial balances combined by hand. | Power Query pulls every entity file into one table; AI writes the steps and explains FX differences. | Power Query + Copilot | Medium |
| VAT review (UAE 5%, KSA 15%) | Checking tax codes, reverse charge on imported services, missing TRNs. | Scans the invoice listing for wrong tax codes, missing TRN, reverse-charge candidates. | Copilot in Excel | Easy |
| E-invoicing readiness (2027) | Customer and vendor masters with missing or messy TRNs, addresses and IDs. | Cleans and validates master data; drafts the readiness checklist and supplier communications. | Copilot in Excel, Power Query | Easy |
| Accounts payable | Keying vendor PDF invoices into the ERP. | Reads the PDF, extracts vendor, TRN, date, amount, VAT; routes for approval. | Power Automate + AI Builder | Medium |
| Collections (AR) | Long payment cycles with government and enterprise clients; chasing by email in two languages. | Drafts polite, firm reminders in English and Arabic; prioritises by ageing and amount. | Copilot in Outlook, Collections agent | Easy |
| Month-end variance commentary | Writing "why did cost go up" for 40 cost centres. | First draft of commentary from the variance table and your notes. You edit. | Copilot in Excel/Word | Easy |
| Corporate tax workpapers | Identifying non-deductible items (e.g. 50% entertainment) across the GL. | Flags GL lines whose descriptions suggest disallowable expenses for your review. | Copilot in Excel | Medium |
| Audit PBC requests | Answering auditor queries, assembling evidence. | Drafts responses from your notes, builds the PBC tracker, summarises supporting docs. | Copilot in Word/Excel | Easy |
| Management reporting pack | Rebuilding the same PowerPoint each month. | Turns the Excel summary into slides with narrative; Power BI answers questions in plain English. | Copilot in PowerPoint, Power BI | Advanced |

### What is changing in the UAE right now

E-invoicing · Peppol PINT AE

#### PDF invoices are being replaced by structured data

Businesses with annual revenue of AED 50 million or more must appoint an Accredited Service Provider by 30 October 2026 and go live on 1 January 2027. Those below that threshold follow on 1 July 2027, and government entities on 1 October 2027. Penalties include AED 5,000 per month for failing to implement or appoint an ASP.

Moving from posting letters to sending bank transfers: the invoice becomes data a machine reads instantly, which is exactly what AI and automation need.

Corporate tax · 9%

#### A new annual workpaper cycle

Returns and payment are due within nine months of the tax period end, so a December 2025 year-end was due by 30 September 2026. Records must be kept for at least seven years. Every recurring, rule-based review here is a candidate for AI-assisted first pass.

A new annual statutory audit you now run in-house: the second year is always faster if you systemise the first.

### Real-world evidence

Gartner · 2025

#### 59% of finance functions use AI

Up from 37% in 2023, based on a survey of 183 CFOs and senior finance leaders. Optimism grows as teams get more hands-on experience.

McKinsey · 2025

#### 88% of organisations use AI somewhere

But nearly two-thirds have not scaled it. The companies getting real value redesign the workflow around AI instead of bolting it on.

Roland Berger · case study

#### 24% less manual AP effort

A global automotive manufacturer identified this saving by combining process clean-up with automation and AI. Standardise first, then automate.

03

Module 03 · 30 minutes

## Your toolkit

Your company licenses and allows Microsoft 365 Copilot, so it is your main AI tool from day one. It runs under your company login, keeps data inside the corporate Microsoft environment, and is the right place for real financial and client data. Power Automate, AI Builder and the Finance agents are separate add-ons; check with IT whether those are enabled before rungs 4 and 5.

### The automation ladder: climb one rung at a time

1

#### AI chat assistant

Microsoft 365 Copilot Chat, or your company's approved ChatGPT/Claude/Gemini. Ask questions, draft, summarise.

Day 1\
Available now

2

#### Copilot inside Excel, Outlook, Word, Teams

AI that sees the file or email you have open: "highlight duplicates", "summarise this thread", "draft a reply".

Week 1\
Available now

3

#### Power Query

Built into Excel. Records your data-cleaning steps once and replays them every month. AI writes the steps for you.

Weeks 2–3\
Free in Excel

4

#### Power Automate + AI Builder

"When an email with an invoice arrives, read it, save it, log it, ask for approval." Runs without you.

Weeks 4–6\
May need IT approval

5

#### Finance agents

Copilot's Financial Reconciliation and Collections agents run reconciliations and AR follow-up on a schedule.

Month 2+\
With IT/finance systems team

Learning to cook. First you follow a recipe card (chat), then use a food processor (Copilot in Excel), then batch-cook for the week (Power Query), then hire a kitchen that cooks every day without you (Power Automate and agents).

### Tool cards

#### Microsoft 365 Copilot

Approved · start here

**Best for:** summarising Teams meetings and email threads, drafting in Word, analysing tables in Excel, building PowerPoint from a document.

**Why first:** works under your company's Microsoft login, so data stays within the corporate tenant.

**Try:** in Excel, format your data as a table (Ctrl+T), open Copilot, ask "Show the top 10 vendors by spend and any vendor that appears under two different names."

#### Copilot Finance agents

Reconciliation

**Best for:** matching two data sets in Excel (bank vs GL, intercompany A vs B, sub-ledger vs GL).

**How it works:** suggests matching rules, maps key and amount columns, then reports perfectly matched, potentially matched and unmatched items. Can run on a schedule.

**Learn:** [Microsoft Learn: reconciliation overview](https://learn.microsoft.com/en-us/copilot/finance/reconcile/reconcile-overview)

#### Power Automate + AI Builder

Automation

**Best for:** invoice intake, approval routing, scheduled reports, reminder emails.

**Key feature:** the prebuilt "Extract information from invoices" model reads PDFs and gives each field a confidence score, so low-confidence items go to a human.

**Learn:** [Microsoft Learn module (free)](https://learn.microsoft.com/en-us/training/modules/ai-builder-invoice-processing/)

#### Power Query (Excel)

Free, underrated

**Best for:** combining 12 entity trial balances, cleaning ERP exports, unpivoting reports.

**AI angle:** ask Copilot or ChatGPT "write the Power Query M code to…" and paste it into the Advanced Editor.

**Learn:** [Power Query documentation](https://learn.microsoft.com/en-us/power-query/)

#### Power BI with Copilot

Later

**Best for:** project profitability and DSO dashboards that management can query in plain English.

**When:** once your data is clean through Power Query, usually month 2 or 3.

#### ChatGPT, Claude, Gemini

Policy check

**Best for:** learning, research, formula help, drafting with no confidential data.

**Rule:** Copilot is your approved tool, so all company and client data goes there. Use free consumer chatbots only for general learning with public information, unless IT approves them too.

04

Module 04 · 60 minutes, the most important module

## How to brief the AI

Prompting is delegation. The skills that make you good at briefing a junior (context, clear deliverable, an example, a deadline) make you good at prompting. Most bad AI output comes from a one-line brief.

### The R-T-C-F-E-C brief

R

Role

Who should it act as? "A senior IFRS accountant"

T

Task

The exact deliverable. "Draft variance commentary"

C

Context

Company, period, currency, audience, the data

F

Format

Table, bullets, word limit, tone

E

Example

Paste last month's good version

C

Check

"List assumptions and anything you're unsure of"

ICAEW teaches a very similar five-part structure (Task, Persona, Context, Example, Format) in its generative AI courses for accountants. The extra "Check" step here forces the AI to tell you where it might be wrong.

Weak brief

```
Explain the variance in IT costs.
```

Result: generic textbook paragraph about IT costs. Useless.

Strong brief

```
You are a finance business partner at an IT services company in Dubai.
Task: draft variance commentary for Sept 2026 vs budget for the CFO.
Context: Software licences AED 412k vs budget 330k (+82k). Notes: Microsoft EA true-up 55k booked in Sept; 12 new delivery consultants onboarded for the Riyadh bank project, each needing licences.
Format: 3 bullet points, max 60 words, state whether one-off or recurring.
Check: list any assumption you made.
```

Result: specific, ready to edit in under a minute.

**Five habits that double the quality:**

- **Iterate.** Treat the first answer as a draft: "shorter", "more formal", "add a column for VAT".
- **Give it the document.** Attach the contract or table rather than describing it.
- **Ask for its working.** "Show step by step how you reached this."
- **Ask it to interview you.** "Before you start, ask me up to five questions you need answered."
- **Save your best prompts** in a OneNote page. Your prompt library is a personal asset.

### Prompt library for your role

Tap a prompt to open it, then copy and replace anything in \[brackets\]. Only paste company data into your company-approved tool.

05

Module 05 · 2 hours per recipe

## Five automation recipes

Each recipe is a real, buildable workflow. Do them in order: each one teaches a skill the next one uses. Before automating anything, apply the accountant's rule: a messy process automated is just a faster mess. Standardise first.

Recipe A · Copilot in Excel

### Variance commentary in ten minutes instead of two hours

EasySaves \~2 hrs/month

Budget vs actual table*→*Copilot flags material lines*→*You add 1-line reasons*→*Copilot drafts narrative*→*You review & send

1. Export budget vs actual by cost centre into Excel. Select the data and press **Ctrl+T** to make it a table (Copilot works best on tables).
2. Open Copilot and ask: "Add a column for variance in AED and %, then highlight rows where the variance exceeds AED 25,000 or 10%."
3. Add a "Notes" column and type a few words of the known reason for each highlighted row (e.g. "EA true-up", "new hires Riyadh").
4. Use the variance commentary prompt from Module 04 with the table attached. Ask for one bullet per highlighted line.
5. Check every number in the commentary against the table. Edit tone. Save the final as next month's "Example" for the prompt.

Recipe B · Power Query

### Combine all GCC entity trial balances with one click

MediumSaves \~4 hrs/month

One folder of TB exports*→*Power Query "From Folder"*→*Add entity + FX rate*→*One AED table*→*Refresh next month

1. Create a SharePoint or OneDrive folder. Save each entity's trial balance export (UAE, KSA, Qatar, Kuwait, Oman, Bahrain) with the same column layout and the entity code in the file name.
2. In Excel: **Data → Get Data → From File → From Folder**. Choose the folder, then **Combine & Transform**.
3. Make a small table of month-end FX rates to AED and merge it in on the currency column. Add a column: Amount × Rate.
4. Stuck on a step? Ask Copilot: "Write Power Query M code that extracts the entity code from the Source.Name column, which looks like TB_KSA01_2026-09.xlsx."
5. Load to a sheet and pivot. Next month, drop new files in the folder and press **Refresh All**. Every step replays.

Recording a macro for your data cleaning, except it is readable and rarely breaks.

Recipe C · Copilot Financial Reconciliation agent

### Bank or intercompany reconciliation, matched by AI

MediumSaves \~6–8 hrs/month

Bank statement*+*GL cash export*→*Agent suggests rules*→*Matched / possible / unmatched*→*You clear exceptions

1. Confirm with IT that the Finance agents add-in is enabled for your Microsoft 365 licence.
2. Put the bank statement and the GL cash ledger as two tables in one workbook (or two sheets).
3. Open the Finance agents panel in Excel and start a reconciliation. Review the suggested key columns (reference, date) and amount columns. Adjust tolerance for bank charges if needed.
4. Read the report: perfectly matched items need a glance; "potentially matched" need your judgement; unmatched become your reconciling items.
5. Once you trust the rules (after 2–3 months), save them as a template and set a recurring run so it is ready on working day 1.

Recipe D · Power Automate + AI Builder

### Vendor invoices read and logged automatically

MediumSaves \~10 hrs/month

Email to ap@ inbox*→*Save PDF to SharePoint*→*AI Builder extracts fields*→*Row added to Excel log*→*Low confidence → you

1. Ask IT for Power Automate access and AI Builder credits (often bundled with premium licences). Agree a shared mailbox or folder for invoices.
2. In Power Automate, create an **Automated cloud flow** with the trigger "When a new email arrives (V3)", filtered to "has attachments".
3. Add "Create file" to save each PDF to a SharePoint library, then the AI Builder action **Extract information from invoices** on that file.
4. Add "Add a row into a table" to write vendor, TRN, invoice number, date, net, VAT and total into an Excel log.
5. Add a condition: if any confidence score is below 0.80, or the TRN is blank, send yourself a Teams message to review. Otherwise route for approval.
6. Run it in parallel with your manual process for one month and compare. Only then switch over.

This recipe also prepares you for e-invoicing, which delivers invoices as structured data from 2027. Your log and approval flow will carry straight across.

Recipe E · Copilot in Outlook + Power Automate

### Weekly collections chasers, prioritised and drafted

EasySaves \~3 hrs/month

AR ageing export*→*Copilot ranks by risk*→*Drafts EN / AR emails*→*You approve*→*Monday reminder

1. Each Monday, export AR ageing. Ask Copilot in Excel: "List customers over 90 days or over AED 100,000 outstanding, sorted by amount, with their oldest invoice."
2. Use the collections prompt from Module 04 to draft emails. For Arabic-speaking contacts, ask for a bilingual version.
3. Review tone carefully for key government and enterprise clients, then send from your own mailbox.
4. In Power Automate, create a **Scheduled cloud flow** every Monday 08:00 that posts a Teams reminder with a link to the ageing file. Small nudge, big habit.

### Estimate your own time savings

Enter your real hours per month. The "saving %" defaults are conservative starting estimates for planning only; replace them with what you measure after a month of use.

06

Module 06 · 20 minutes

## Controls: using AI without getting burned

Accountants already have the right instincts: segregation of duties, evidence, review. Apply exactly those to AI.

#### 1. Know where the data goes

Your company's Microsoft 365 Copilot keeps prompts inside your organisation's Microsoft environment, so use it for work data. Free consumer chatbots may not. Never paste client names, contract values, salaries or bank details into any tool other than Copilot.

Sending a confidential file by company email versus a personal Gmail.

#### 2. Every number gets ticked

AI can produce totals that look right and are not. Do calculations in Excel; use AI to write the formula, not to be the formula. Reconcile AI-produced schedules back to the GL.

#### 3. Cite the source, not the AI

For tax and IFRS positions, ask AI to point you to the relevant standard or FTA guide, then read the original. Your working paper cites the FTA, never "ChatGPT said".

#### 4. Keep an audit trail

For automated flows, log what was processed, by which flow, and who approved. Auditors will ask how an automated control works and who reviews exceptions.

#### 5. Respect privacy law

The UAE Personal Data Protection Law (Federal Decree-Law No. 45 of 2021) and your employer's global policies apply to employee and customer personal data. Strip or mask personal details before analysis where you can.

#### 6. Ask first, then build

Before building any automation that touches the ERP or bank, show it to your manager and IT. In a large company, a shadow automation that breaks at year-end is a career risk; an approved one is a promotion story.

**Red lines.** Do not let AI post journals, approve payments, change vendor bank details, or file tax returns without a human approval step. Treat any email asking to change bank details as fraud until verified by phone; AI makes such emails far more convincing.

07

Module 07 · your 8-week plan

## From first prompt to first automation

About 2–3 hours a week. Tick items as you go; your progress is saved in this browser.

0%

**Week 8 deliverable:** a one-page note to your manager: what you automated, hours saved per month (from the calculator, now with measured numbers), controls in place, and the next process you propose. This is how individual experiments become recognised team practice.

08

Module 08 · reference library

## Videos, courses, guides and research

Hand-picked, in the order a beginner should take them. Start with anything marked "Start here".

Prepared October 2026. Product features, licences and UAE regulations change; confirm current details with your IT team, Microsoft Learn and the Federal Tax Authority before acting. Savings figures are illustrative planning estimates, not guarantees.