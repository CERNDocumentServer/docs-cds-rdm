# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **MkDocs Material** user documentation site for CDS (CERN Document Server). The site uses modern Python tooling with **uv** for dependency management, Markdown for content, and Material for MkDocs theme for beautiful, responsive design.

## When applying changes

- Limit emojis: this is a user documentation that should be kept professional.
- Explain concepts and how-to use features in a clear and concise way. Screenshots should be always kept.
- When you review the text of a page, limit the changes to the page structure and limit the number of sections.

## Development Commands

**Install dependencies:**

```bash
uv sync
```

**Start local dev server with hot reload:**

```bash
uv run mkdocs serve
```

**Build static site:**

```bash
uv run mkdocs build
```

## Technology Stack

- **MkDocs Material**: Beautiful documentation theme
- **uv**: Fast Python package manager
- **Python 3.12+**: Runtime environment
- **Markdown**: Content format

## Key Files

- **`mkdocs.yml`**: MkDocs configuration
- **`pyproject.toml`**: Python dependencies
- **`docs/`**: All documentation source files
- **`site/`**: Generated static site (git-ignored)
