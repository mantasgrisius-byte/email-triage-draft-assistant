# Project #02: Email Triage & Draft-Reply Assistant

**Status:** New — not started yet

## Business problem

Small and mid-size service businesses (beauty salons, real-estate agencies, e-commerce shops) get dozens to hundreds of emails a day — questions, complaints, orders. Staff waste time sorting them manually, and important emails sometimes get lost among routine ones.

## Automation solution

The system reads incoming emails, classifies them by type and urgency, drafts a reply for a human to approve or edit, and immediately escalates urgent or complex cases to the responsible person with a summary.

## Tech stack

- Gmail/Outlook API
- Claude API
- text classification
- draft generation

## Why this project is in the portfolio

A natural next step after Project #1 — reuses the same 'read and understand a document' foundation, but adds a new, immediately visible layer: the AI writes text, not just extracts data.

## Important

- This project is built with **fake (synthetic)** data, not real client data — the
  demo must be safe to show to anyone, at any time.
- The AI component must never invent missing data — when something is missing or
  unclear, the system must flag it for human review instead of guessing.
