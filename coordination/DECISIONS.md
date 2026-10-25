# Decision register

Record the decision, status, date, decision-maker, rationale, scope, alternatives, and evidence. Keep operator choices distinct from routine implementation choices and unapproved research proposals. Append a supersession note when a choice changes.

## D-001: Establish the research foundation

- Date: 2026-10-25.
- Status: operator-approved scope.
- Decision-maker: operator, in the current task request.
- Choice: set up AmericanFutureSocietyProject with the full vision, research departments, READMEs, and shared agent log.
- Rationale: preserve context and build a serious research basis before treating brainstorms as conclusions.
- Scope: repository foundation. This does not adopt economic promises, a site, legal structures, investments, technologies, or continuing work.
- Record: [AFS-0001](tasks/AFS-0001-foundation.md).

## D-002: Keep the initial foundation in plain Markdown

- Date: 2026-10-25.
- Status: implementation choice within D-001; revisable.
- Decision-maker: implementing agent.
- Choice: linked Markdown charters, registers, and templates; a separate digital-twin specification; no new runtime dependencies or automatic orchestration.
- Rationale: easy to inspect in GitHub, portable across AI tools, and sufficient for the requested organizational work.
- Alternatives: a database or agent platform would add setup and operational commitments before the research needs them; a single large README would make specialist context and handoffs difficult to maintain.

## D-003: Preserve the licensing decision

- Date: 2026-10-25.
- Status: open operator decision.
- Question: what reuse terms should apply to prose, datasets, code, and outside contributions?
- Current treatment: no license selected; see [license status](../LICENSE-STATUS.md).

## D-004: Public publication

- Date: 2026-10-25.
- Status: operator-approved.
- Observation: GitHub reports the repository public.
- Decision-maker: operator, explicitly approving "Publish the foundation and integrate into main" in reply to the publication request.
- Choice: publish the reviewed foundation to `SlipstreamAI/AmericanFutureSocietyProject` and integrate it into `main`.
- Scope: this foundation and its publication records. Repository visibility, licensing, future research, outreach, and deployment are separate decisions.
- History: preparation was held locally until this approval was received; that publication blocker is now resolved.
- Publication and integration record: [PR #1](https://github.com/SlipstreamAI/AmericanFutureSocietyProject/pull/1).
