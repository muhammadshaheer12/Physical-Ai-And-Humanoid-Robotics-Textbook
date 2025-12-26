# ADR-0002: Content Management Strategy

> **Scope**: Document decision clusters, not individual technology choices. Group related decisions that work together (e.g., "Frontend Stack" not separate ADRs for framework, styling, deployment).

- **Status:** Proposed
- **Date:** 2025-12-26
- **Feature:** 4-climate-policy-paper
- **Context:** The research paper requires a method for storing content and managing academic citations. The content will be written in Markdown and needs to support APA citation style.

<!-- Significance checklist (ALL must be true to justify this ADR)
     1) Impact: Long-term consequence for architecture/platform/security?
     2) Alternatives: Multiple viable options considered with tradeoffs?
     3) Scope: Cross-cutting concern (not an isolated detail)?
     If any are false, prefer capturing as a PHR note instead of an ADR. -->

## Decision

- **Content Storage**: Markdown files (`.md`)
- **Citation Management**: A dedicated citation manager (e.g., Zotero) is recommended.

<!-- For technology stacks, list all components:
     - Framework: Next.js 14 (App Router)
     - Styling: Tailwind CSS v3
     - Deployment: Vercel
     - State Management: React Context (start simple)
-->

## Consequences

### Positive

- Markdown is a simple, plain-text format that works seamlessly with Docusaurus and version control.
- Using a citation manager automates the tedious process of formatting citations and bibliographies, ensuring accuracy and consistency.

### Negative

- Complex tables or layouts can be challenging in standard Markdown.
- Integration between the citation manager and the Docusaurus build process may require custom scripting.

## Alternatives Considered

- **Alternative A: Headless CMS**: Using a headless CMS would provide a richer editing experience but adds significant complexity and a database dependency.
- **Alternative B: Manual Citation Management**: Manually formatting citations is error-prone and time-consuming.

## References

- Feature Spec: `specs/4-climate-policy-paper/spec.md`
- Implementation Plan: `specs/4-climate-policy-paper/plan.md`
- Related ADRs: `history/adr/0001-authoring-and-deployment-technology-stack.md`
- Evaluator Evidence: None
