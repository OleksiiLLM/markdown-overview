# 3. GitHub Flavored Markdown (GFM)

## What is it?
GitHub Flavored Markdown (GFM) is the specific dialect (superset) of Markdown used for user content on GitHub.com and GitHub Enterprise. 

## The Relationship to CommonMark
GFM is a **strict superset** of the CommonMark specification. This means that everything that is valid in CommonMark behaves exactly the same way in GFM. 

## Why was it needed?
While CommonMark standardizes the core features of Markdown (like paragraphs, lists, bold text, and links), developers and writers on GitHub needed additional, specific features for collaboration, documentation, and code sharing that were not part of the original Markdown or CommonMark specs.

GFM adds these features as **extensions** on top of CommonMark.

## Key GFM Extensions:
*   **Tables:** Allows for the creation of data tables using pipes (`|`) and hyphens (`-`).
*   **Task List Items:** Allows lists to have renderable checkboxes (e.g., `- [x] finished task`).
*   **Strikethrough:** Allows text to be struck through using tildes (e.g., `~~strikethrough~~`).
*   **Autolinks Extension:** Automatically recognizes raw URLs (like `http://example.com` or email addresses) without requiring them to be wrapped in angle brackets (`< >`).
*   **Disallowed Raw HTML:** For security and layout consistency, GFM filters out specific raw HTML tags (like `<script>`, `<style>`, `<iframe>`, `<title>`) by replacing their leading `<` with `&lt;`, preventing them from executing or breaking the page layout.
