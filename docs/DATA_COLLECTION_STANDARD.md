# UP Election Atlas — Data Collection Standard (Version 1.0)

## Purpose

This document defines the official rules for collecting, storing, verifying, updating, and publishing data within the UP Election Atlas project.

Every dataset, constituency profile, candidate profile, election result, and AI-generated summary must comply with these standards.

---

# Core Principles

1. Facts over opinions.
2. Every fact must be verifiable.
3. Never fabricate information.
4. Never estimate missing values.
5. Missing information should be stored as null.
6. AI analysis must always remain separate from factual data.
7. Every important value must be traceable to its original source.

---

# Source Hierarchy

## Tier 1 (Highest Priority)

- Election Commission of India (ECI)
- Census of India
- Government of Uttar Pradesh
- Parliament / Vidhan Sabha
- National Informatics Centre (NIC)

These sources always take precedence.

---

## Tier 2

- ADR / MyNeta
- PRS India
- RBI
- NITI Aayog
- Ministry Dashboards

---

## Tier 3

- IndiaStat
- CSDS
- CMIE
- Government Open Data Portals

---

## Tier 4

National newspapers.

Examples:

- The Hindu
- Indian Express
- Hindustan Times
- Times of India

---

## Tier 5

Regional newspapers.

Use only when higher-quality sources are unavailable.

---

## Tier 6

Wikipedia

Wikipedia may be used only to discover information or locate primary sources.

Wikipedia should never be the final authority if an official source exists.

---

# Data Rules

Never guess.

Never extrapolate.

Never calculate demographic values that have not been officially published.

If data cannot be verified:

Use

null

Never use:

Unknown

Approximate

Estimated

Likely

Probably

---

# Dates

Always use ISO format.

YYYY-MM-DD

Example

2027-02-10

---

# Currency

All money should be stored in Indian Rupees.

No commas.

Correct

12500000

Incorrect

1,25,00,000

---

# Percentages

Store percentages as numbers.

Correct

56.81

Incorrect

"56.81%"

---

# Coordinates

Latitude

Longitude

Decimal format only.

---

# Candidate Names

Always use the official affidavit spelling.

---

# Party Names

Use the official Election Commission name.

Reference by party_id whenever possible.

---

# Constituencies

Use the official Assembly Constituency Number.

Example

174-lucknow-central

Never rename constituencies.

---

# Missing Data

If a value cannot be verified

Store

null

Do not remove the field.

---

# AI Generated Content

AI may generate:

- summaries
- insights
- trend analysis
- political narratives
- swing probability

AI must never generate:

- fake statistics
- fake turnout
- fake demographics
- fake quotations
- fake news

All AI output must clearly state it is analytical and not factual.

---

# News

Only paraphrase.

Never copy articles.

Always include

headline

publisher

publication date

URL

retrieved date

---

# Citations

Every important value should include

- source_id
- retrieved_date
- confidence

---

# Version Control

Every dataset should contain

schema_version

dataset_version

last_updated

last_verified

---

# Repository Philosophy

UP Election Atlas is not a prediction platform.

It is not affiliated with any political party.

It exists to build the most accurate, transparent and structured election knowledge base for Uttar Pradesh.

Accuracy is always more important than completeness.
