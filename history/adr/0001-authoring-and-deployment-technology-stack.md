# ADR-0001: Authoring and Deployment Technology Stack

> **Scope**: Document decision clusters, not individual technology choices. Group related decisions that work together (e.g., "Frontend Stack" not separate ADRs for framework, styling, deployment).

- **Status:** Proposed
- **Date:** 2025-12-26
- **Feature:** 4-climate-policy-paper
- **Context:** The project requires a toolchain for authoring a research paper and deploying it as a static website. The target audience is undergraduate economics students.

<!-- Significance checklist (ALL must be true to justify this ADR)
     1) Impact: Long-term consequence for architecture/platform/security?
     2) Alternatives: Multiple viable options considered with tradeoffs?
     3) Scope: Cross-cutting concern (not an isolated detail)?
     If any are false, prefer capturing as a PHR note instead of an ADR. -->

## Decision

- **Authoring**: Spec-Kit Plus
- **Deployment**: Docusaurus

<!-- For technology stacks, list all components:
     - Framework: Next.js 14 (App Router)
     - Styling: Tailwind CSS v3
     - Deployment: Vercel
     - State Management: React Context (start simple)
-->

## Consequences

### Positive

- Spec-Kit Plus provides a structured authoring workflow.
- Docusaurus is a mature and well-supported static site generator, ideal for documentation-style websites.
- The combination allows for rapid development and deployment.

### Negative

- Docusaurus is primarily designed for software documentation, not academic papers, so some features may not be a perfect fit.
- Using Spec-Kit Plus introduces a dependency on a specific toolchain.

## Alternatives Considered

- **Alternative A: LaTeX + PDF**: Traditional academic publishing format. Rejected because web-based output is desired.
- **Alternative B: Hugo/Jekyll + Markdown**: Other static site generators. Docusaurus was chosen due to existing project familiarity.

## References

- Feature Spec: `specs/4-climate-policy-paper/spec.md`
- Implementation Plan: `specs/4-climate-policy-paper/plan.md`
- Related ADRs: None
- Evaluator Evidence: None
