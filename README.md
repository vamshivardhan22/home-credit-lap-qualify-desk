# Home Credit LAP — Qualify Desk

Public notes for the SalesAgents AI voice-agent assignment (Vamshi Vardhan).

## What was built

Qualify Desk is a working rehearsal app for Home Credit's Loan Against Property qualifier. It implements the assignment rules, not a yes/no script.

- Call floor: reply as the customer. The checklist updates as facts arrive, including facts given out of order.
- The call stops immediately on agricultural property, cash income, missing originals, tenure outside 3–15 years, an existing loan or EMI-reduction request, or a request above ₹75 lakh that the customer refuses.
- Above ₹75 lakh, the agent offers the ₹75 lakh cap and continues only if accepted.
- Handoff to a senior loan expert happens only after all 7 points pass. No invented interest rate, fee, branch, or minimum property value.
- System prompt with the required variables (`customer_name`, `agent_name`, `agent_gender`, `language_to_speak`, date/day/time, `additional_context_from_rag`, utterance, history), copy-ready for Retell or Bolna. Hindi gender agreement is specified.
- Scenario lab with expected outcomes and reference transcripts.
- Approach write-up of the easy-to-miss rules.
- 35 automated tests on the qualification engine.

## GitHub

- This public repo: https://github.com/vamshivardhan22/home-credit-lap-qualify-desk
- Full app export (private workspace repo): https://github.com/vamshivardhan22/lilac-sage-lunar-wave

## How a clean file sounds

1. Yes, this is Rahul.
2. Yes, please go ahead.
3. It's a residential flat worth about 1 crore, and I'm the sole owner.
4. Yes, the original documents are at home.
5. I need 50 lakh.
6. I'm salaried and my salary comes into my bank account.
7. I'd like 10 years.

Expected result: senior loan expert handoff. Saying the property is agricultural land after the offer ends the call at once.
