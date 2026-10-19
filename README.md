# Home Credit LAP — Qualify Desk

Qualify Desk is a small web application and qualification-engine demo built for a Loan Against Property (LAP) voice-agent assignment. It applies defined business rules to a customer conversation and records whether the case can continue, should be transferred, or must end.

## What it covers

- Captures seven core qualification areas: property type, ownership, availability of original documents, requested loan amount, occupation and income mode, property market value, and tenure.
- Tracks responses even when a customer provides details out of order.
- Handles disqualification conditions such as agricultural property, unavailable original documents, cash income, and tenure outside the configured 3–15 year range.
- Offers a capped amount where the requested loan exceeds ₹75 lakh and continues only if the customer accepts.
- Routes existing-loan or EMI-reduction requests to a senior loan expert.
- Includes a scenario lab and reference transcripts for testing call outcomes.
- Includes automated tests for the qualification engine.

## Technology

- TypeScript
- React
- TanStack Router / Start
- Vite
- Zod
- Automated tests

## Repository links

- [Qualify Desk application](https://github.com/vamshivardhan22/lilac-sage-lunar-wave)
- [Related qualification demo](https://github.com/vamshivardhan22/fjord-daisy-nova-hill)

## Run locally

Requirements: Node.js and npm.

```bash
git clone https://github.com/vamshivardhan22/home-credit-lap-qualify-desk.git
cd home-credit-lap-qualify-desk
```

The repository currently contains the assignment README and supporting notes. To run the interactive application, use the linked application repository above and follow its project setup instructions.

## Important note

This project demonstrates rule-based qualification and call handling. It is not a credit decision system and does not replace formal lender underwriting. Confirm all thresholds and eligibility rules with the lender before any operational use. Do not put real customer information into a public demo.
