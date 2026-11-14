---
name: sqlp-learning
description: Explain SQL and database concepts through focused conversation, correct the user's stated understanding at the same level, and preserve each completed topic as a sequential HTML learning page in this project.
metadata:
  short-description: SQL learning notes for this project
---

# SQL Learning

Use this skill when the user discusses SQL, database internals, query processing, or asks to preserve a learning conversation in the project.

## Explanation scope

- Treat the user's description as a draft understanding: confirm what is right, then correct only the parts that are materially inaccurate.
- Keep the explanation at the level of the user's wording and current question. Define only the terms needed to resolve the confusion; do not turn a short question into a broad tutorial.
- State the database product or version when behavior is product-specific. If it is unclear and affects correctness, explain the assumption briefly or ask one focused question.
- For niche or version-sensitive behavior, verify with authoritative sources and link sources near the relevant claim. Separate general concepts from product-specific details.
- Keep diagrams and examples small and directly tied to the question.

## Preserve a completed conversation

At the end of a learning conversation, create one standalone HTML page for the SQL concepts covered in that conversation. Before writing:

1. Inspect the existing documentation structure and style. Reuse its document shell, CSS, typography, section patterns, and navigation conventions where available. Do not copy another project's implementation assets into this project without a reason.
2. Find the next sequence number from existing learning pages and sidebar entries. Create exactly one new page for the completed conversation; keep earlier pages intact.
3. Write a concise Korean note that preserves the question's scope: the corrected mental model, a short explanation, and sources when needed. Do not reproduce every chat turn.
4. Add the new page as the next item in the left navigation, in chronological order. Update the shared index/navigation page if the project uses one, and keep the navigation consistent on all generated learning pages.
5. Check all local links, page titles, and sequence numbers. Show the finished HTML page to the user when practical.

## Print-ready output

- Every standalone learning page, including the shared index, must remain printable and PDF-friendly. Add print styles that hide navigation, use a white background with readable contrast, expand the content column, wrap long code and URLs, and allow the full body to paginate.
- Keep headings with the content that follows. Do not let fixed dimensions, scroll containers, or screen-only backgrounds clip or hide material in print.
- When adding or changing print styles, inspect print preview or an exported PDF for complete body content, margins, page breaks, and readable code or tables. Report when visual print inspection is unavailable.

If no documentation structure exists yet, create a small `docs/learning/` collection with an `index.html` and numbered topic pages such as `001-sql-processing.html`. Use a shared left sidebar on the index and each topic page, with entries ordered by sequence number. Keep the visual treatment close to the project's other documentation: a persistent left navigation, a centered readable content column, a clear page title, short purpose text, structured sections, and restrained callout styling.
