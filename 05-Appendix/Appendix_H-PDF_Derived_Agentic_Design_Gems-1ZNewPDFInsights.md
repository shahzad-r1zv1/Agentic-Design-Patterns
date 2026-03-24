# Appendix H: Agentic Design Gems from Recent Research (2025-2026)

This appendix distills patterns and ready-to-use ideas from the PDFs in the main folder. Each subsection summarizes a paper and translates its “gems” into concrete design hooks you can drop into chapters or implementations.

## Human–Agentic SDLC Security (Ayouni et al., 2026)
- **DevSecOps copilot loop:** Pair agentic scanners (breadth) with human reviewers (risk acceptance); route “low-risk” findings for escalation when blast radius is high.
- **Context-aware triage:** Combine historical exploit data with forward-looking heuristics; trigger live human review when impact > threshold even if likelihood is low.
- **Regulatory alignment:** Keep a policy registry the agent checks before auto-patching; block actions lacking mapped compliance controls.

## Worker–Supervisor Split for Scientific Agents (Baibakova & Serov, 2026)
- **Split-brain pattern:** Small fine-tuned worker generates tool code; large supervisor validates outputs and rewrites prompts only when drift/hallucination risk rises.
- **Energy-aware orchestration:** Prefer the worker; call the supervisor sparingly with hard gates (quality checks, symmetry/constraint validators) to cut cost by design.
- **Dataset curation loop:** Build parsers to serialize tool outputs for automatic structural checks before user-visible responses.

## Ethics Beyond Asimov (Bozkurt, 2025)
- **Dynamic guardrails:** Codify organization-specific “laws” as policies; agents must surface the policy match for every high-impact action.
- **Human agency preservation:** Fast overrides, pause/stop buttons, and audit trails as first-class features to avoid opaque delegation creep.

## S5 Sustainable Design Framework (Maldonado-Romo et al., 2026)
- **Multi-agent by dimension:** Sensing, Smart, Sustainability, Social, Safe agents with shared traceability across digital/physical twins.
- **Lifecycle dashboards:** Track optimization, risk, and environmental KPIs per dimension; gate releases on cross-dimension consensus.
- **Case pattern:** Use for robotics/IoT where physical safety, sustainability, and social acceptability must co-evolve.

## Four-Phase Autonomy Loop (Pati, 2025)
- **Loop:** Data collection → decision → learning → collaboration.
- **Fleet sharing:** Sync near-miss learnings, reroutes, and policy updates across agents; adds resilience and consistency.
- **Narrative transparency:** Require agents to explain decisions in user-facing channels to build trust.

## Gen Z Adoption Drivers (Hasselwander & Lah, 2026)
- **Necessary conditions:** Trust, transparency, and user control are prerequisites, not nice-to-haves.
- **UX patterns:** Consent defaults, notice-and-choice on data use, one-tap pause/stop for background agents.
- **Measure adoption:** Instrument satisfaction/trust as leading indicators, not just task completion.

## Healthcare Seven-Dimensional Taxonomy (Vatsal et al., 2026)
- **Self-monitoring:** Agents critique intermediate steps; deferral triggers when evidence weakens.
- **Consensus protocols:** Multi-agent deliberation and sampling-based cross-checks to converge on reliable recommendations.
- **Tool discipline:** Reason–act interleaving (ReAct), API invocation timing, and grounding in clinical knowledge bases.

## DAWN Distributed Architecture (Aminiranjbar et al., 2025)
- **Principal + gateway agents:** Principal plans and orchestrates; gateway agents expose localized resources with data residency boundaries.
- **Execution graphs:** User-approved graphs for traceability; make plans restartable and auditable.
- **Data locality by design:** Keep orchestration local/VPC; request remote resources only through gateways.

## Graph RAG for SEL (Fotopoulou et al., 2026)
- **KG-backed provenance:** Domain knowledge graphs plus RAG for explainable, context-safe guidance.
- **Persona agents:** Specialized advisors (teacher, counselor, domain expert) reading from the same KG to avoid drift.
- **Generalize beyond SEL:** Apply to finance/gov/health where provenance and guardrails matter.

## Agentic Software Engineering SLR (Otoum & Elkhalili, 2026)
- **ASE lifecycle:** Autonomous coding → multi-agent refinement → evaluation baselines with threats-to-validity checklists.
- **Evaluation hooks:** Measure autonomy level, collaboration quality, and defect escape rates post-deployment.
- **Process guardrails:** Require human approvals for risky code paths; log rationale for traceability.

## Traceable Ops Scheduling with Simulation (Cirillo et al., 2025)
- **Simulation-in-the-loop:** Generate plans, simulate, and only then execute; keep RAG citations for every operational instruction.
- **Traceability:** Link actions to sources plus simulation outcomes to pass audits in regulated ops.
- **Resilience:** Prefer plans that degrade gracefully when resources drop or constraints change.

## Critical Infrastructure Protection (Yigit et al., 2025)
- **All-hazards playbooks:** Integrate incident response with business continuity; agents should propose both mitigation and continuity steps.
- **Secure-by-design controls:** Mandatory IDS, crypto, provenance logging (blockchain optional), and periodic penetration-style probes.
- **Risk posture as a signal:** Treat real-time posture (scorecards, asset risk) as input to planning and throttling.

