# Decision Framework

Use this reference to choose the appropriate work mode without over-orchestrating.

## Fast Triage

Assess the request along six dimensions:

- **Input volume:** how many documents, messages, records, notes, or sources are involved?
- **Input quality:** are the sources complete, current, and specific enough?
- **Stake:** what happens if the answer is wrong?
- **Audience:** internal note, team draft, executive material, client communication, contract/RFP, or decision support?
- **Perspective count:** does the task need one view or several independent views?
- **Verifiability:** can claims be checked against inputs, external sources, tests, calculations, or explicit criteria?

Do not ask the user for more context unless the answer could change the selected work mode, risk level, or final-use constraints.

## Mode Selection

Choose the lightest safe option:

- **Single-pass:** low input volume, low risk, internal use, clear request.
- **Two-pass:** moderate risk, external or executive-adjacent use, important tone/claim/source review, but limited scope.
- **Cost-aware delegation:** enough volume for worker help, but subtasks are bounded and verifiable.
- **Small role team:** several expert perspectives matter more than raw processing volume.
- **Larger workflow:** many inputs, high stakes, several work packages, independent verification, and final synthesis all matter.

When uncertain, escalate by one level only. Do not jump from single-pass to larger workflow unless the signal is strong.

## Stop / Go / Source Expansion

Use this gate when source gaps matter.

### Stop

Stop and request specific input when:

- the missing information could materially change the main conclusion, recommendation, risk rating, or external usability;
- the missing input can be named concretely;
- the input is realistically obtainable before the work must be used;
- continuing would create false confidence or serious reputational, legal, financial, sales, or project risk.

### Go With Constraints

Proceed with constraints when:

- the gap is not central to the task;
- the missing input is not realistically obtainable in time;
- the gap can be clearly marked as an assumption, risk, or open question;
- the output remains useful for the intended decision or communication;
- the user explicitly asks to proceed with available material.

Use medium visibility by default: state the main constraint near the beginning or in a brief limitations note. Do not over-label every claim unless the material is high-stakes, disputed, or auditable.

### Source Expansion

Use external sources only when the missing information is realistically verifiable outside the user's private context.

Appropriate examples:

- public company facts;
- market or industry context;
- public news, press releases, regulatory filings, public pricing, official documentation;
- publicly verifiable customer/account background.

Do not use external search to infer:

- internal project status;
- non-public client negotiation state;
- internal decision intent;
- private CRM facts;
- private stakeholder positions.

Separate internal-input facts from external-source facts in the final reasoning.

## Sufficient Certainty

Do not require impossible completeness. Business work almost never has 100% information.

The practical question is:

```text
Could the missing information materially change the main answer or its safe use?
```

If yes, stop or proceed with explicit constraints. If no, continue and avoid cluttering the output with peripheral uncertainty.
