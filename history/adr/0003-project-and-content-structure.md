# ADR-0003: Project and Content Structure

> **Scope**: Document decision clusters, not individual technology choices. Group related decisions that work together (e.g., "Frontend Stack" not separate ADRs for framework, styling, deployment).

- **Status:** Proposed
- **Date:** 2025-12-26
- **Feature:** 4-climate-policy-paper
- **Context:** The new research paper content needs a designated location within the existing `robotics-ai-book` Docusaurus project. The goal is to integrate the new content logically without disrupting the existing site structure.

<!-- Significance checklist (ALL must be true to justify this ADR)
     1) Impact: Long-term consequence for architecture/platform/security?
     2) Alternatives: Multiple viable options considered with tradeoffs?
     3) Scope: Cross-cutting concern (not an isolated detail)?
     If any are false, prefer capturing as a PHR note instead of an ADR. -->

## Decision

- The research paper content will be housed within the `robotics-ai-book/docs/` directory.
- The content will be organized into chapter-based Markdown files (e.g., `chapter-1-introduction.md`).

<!-- For technology stacks, list all components:
     - Framework: Next.js 14 (App Router)
     - Styling: Tailwind CSS v3
     - Deployment: Vercel
     - State Management: React Context (start simple)
-->

## Consequences

### Positive

- Leverages the existing Docusaurus project, avoiding the setup of a new site.
- Collocates all documentation-style content, making it easy to manage and deploy together.
- Follows the conventional structure for Docusaurus sites.

### Negative

- If the `robotics-ai-book` project grows to include many unrelated documents, the `docs` directory could become cluttered.

## Alternatives Considered

- **Alternative A: New Docusaurus Project**: Create a separate, standalone site for the research paper. Rejected to reduce overhead and keep all content in one repository.
- **Alternative B: Different Content Directory**: Place the content in a new top-level directory (e.g., `papers/`). Rejected as it would require custom Docusaurus configuration to include the content in the build.

## References

- Feature Spec: `specs/4-climate-policy-paper/spec.md`
- Implementation Plan: `specs/4-climate-policy-paper/plan.md`
- Related ADRs: 
    - `history/adr/0001-authoring-and-deployment-technology-stack.md`
    - `history/adr/0002-content-management-strategy.md`
- Evaluator Evidence: None
