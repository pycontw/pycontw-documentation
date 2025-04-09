# pycontw-documentation

Documentation project for PyCon Taiwan, built with MkDocs.

## Setting Up Development Environment

### Prerequisites

- Python 3.13+
- [uv](https://github.com/astral-sh/uv) - Fast Python package manager and installer

### Installation

1. Clone this repository
   ```bash
   git clone https://github.com/pycontw/pycontw-documentation.git
   cd pycontw-documentation
   ```

2. Install dependencies with uv
   ```bash
   uv sync
   ```

3. Activate the virtual environment
    - Linux/macOS
        ```bash
        source .venv/bin/activate
        ```
    - Windows
        ```
        source .venv\Scripts\activate  # Windows
        ```

4. Install pre-commit hooks
   ```bash
   pre-commit install
   ```

## Development

### Local Documentation Preview

Start a local server to preview the documentation:
```bash
mkdocs serve
```

Then, visit http://127.0.0.1:8000 in your browser.

### Building Documentation

Generate static HTML files:
```bash
mkdocs build
```

The generated files will be located in the `site/` directory.

### Committing Changes

This project uses the [Conventional Commits](https://www.conventionalcommits.org/) specification with Commitizen:

```bash
git add .
cz c
```

Pre-commit hooks will automatically check code formatting and commit messages.

## Project Structure

- `docs/` - Documentation source files
- `mkdocs.yml` - MkDocs configuration file
- `.pre-commit-config.yaml` - Pre-commit hooks configuration

## Contribution Guidelines

1. Fork this repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`cz c` and fill in the commit message)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request
