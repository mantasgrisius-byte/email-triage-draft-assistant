# Email Triage Taxonomy - Project #02

## Business context

- Single business vertical for this demo: an independent real-estate agency.
  Rationale: agencies still handle most inbound email manually, while
  e-commerce support already has many off-the-shelf AI automation tools
  (Gorgias, Zendesk AI, Intercom), making it a less differentiated niche
  for a portfolio piece.
- All data is synthetic (fake) - safe to demo publicly, no real client data.
- The sample email dataset will include both English and Danish emails.

## Categories

1. Property Inquiry - general question about a specific listed property
   (price, size, condition, availability).
2. Viewing Request - request to schedule, reschedule, or cancel a
   property viewing.
3. Offer / Negotiation - a buyer's offer on price or terms, or
   negotiation follow-up.
4. Document Request - request for a contract, floor plan, energy
   performance certificate, or similar document.
5. Complaint - a dissatisfied client (agent responsiveness, process
   delay, incorrect information, etc.).
6. Other - anything that does not fit the categories above (including
   spam/irrelevant messages).

## Urgency levels

SLA-style priority levels, modeled on common help-desk practice
(ITIL / Zendesk-style four-tier system):

- Urgent - respond within ~1 hour. Example: time-critical situation
  (viewing or closing happening today/tomorrow), or a client publicly
  threatening a negative review / escalation.
- High - respond within the same business day. Example: a clearly
  frustrated client, or an issue tied to an imminent viewing/offer.
- Medium - respond within 1-2 business days. Example: a standard
  inquiry or document request with no time pressure.
- Low - respond within about a week. Example: general information
  request, no urgency implied.

## Core rule (from the project brief)

The AI must never invent missing or unclear information (e.g. a
property's exact price, an appointment time). When something is
missing or ambiguous, the system must set `needs_human_review: true`
instead of guessing.
