# CDS documentation website

Documentation website for CERN Document Server (CDS) built with **MkDocs Material**.

## Quick Start

### Prerequisites

Install [uv](https://docs.astral.sh/uv/), install all dependencies:

```bash
uv sync
```

### Development

Start the development server with live reload:

```bash
uv run mkdocs serve --livereload
```

Then open **http://localhost:8000** in your browser.

### Build

Build the static site:

```bash
uv run mkdocs build

# Clean build
uv run mkdocs build --clean
```
