# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **MkDocs Material** documentation site for CDS (CERN Document Server). The site uses modern Python tooling with **uv** for dependency management, Markdown for content, and Material for MkDocs theme for beautiful, responsive design.

## Development Commands

**Install dependencies:**
```bash
uv sync
# or
npm install
```

**Start local dev server with hot reload:**
```bash
uv run mkdocs serve
# or
npm run serve
```

**Build static site:**
```bash
uv run mkdocs build
# or
npm run build
```

## Technology Stack

- **MkDocs Material**: Beautiful documentation theme
- **uv**: Fast Python package manager
- **Python 3.8+**: Runtime environment
- **Markdown**: Content format

## Key Files

- **`mkdocs.yml`**: MkDocs configuration
- **`pyproject.toml`**: Python dependencies
- **`docs/`**: All documentation source files
- **`site/`**: Generated static site (git-ignored)
