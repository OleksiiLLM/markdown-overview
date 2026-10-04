# 2. CommonMark

## What is it?
CommonMark is a highly defined, unambiguous specification and a suite of reference implementations for Markdown.

## Why was it needed (The Problem with original Markdown)?
The original description of Markdown's syntax by John Gruber was informal and did not specify the syntax unambiguously. It left many edge cases and interactions between syntax elements undefined. 

Examples of ambiguities included:
*   How much indentation is needed for a sublist?
*   Are blank lines required before block quotes, indented code blocks, or headings?
*   What are the precedence rules when block and inline structures overlap?
*   Can list items contain blank lines, headings, or blockquotes?

Because there was no unambiguous specification, dozens of different Markdown parsers (like the original `Markdown.pl`, Pandoc, Redcarpet, marked) implemented their own interpretations of these edge cases. This divergence meant that a document rendering perfectly on one platform might break or render completely differently on another.

## The Solution
CommonMark was created to specify Markdown syntax completely and unambiguously. It provides a comprehensive set of rules and side-by-side parsing tests to ensure that all conforming parsers behave exactly the same way, eliminating surprises for authors moving between different platforms.
