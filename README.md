# Python Template

Cassidy's opinionated Python template. Enter at your own peril.

## Development

Requires [uv](https://docs.astral.sh/uv/)

Setup: `uv sync --dev`

Lint: `uv run ruff check`

Format: `uv run ruff format`

Type-check: `uv run ty check`

Test: `uv run pytest`

Security audit: `uv audit --preview-features audit`

## Template Setup

To use this template for a new project:

1. **Create a new repository** from this template on GitHub (click "Use this template")

2. **Clone your new repository** and navigate to it

3. **Update project metadata** in `pyproject.toml`:
   - Change `name` to your project name (use kebab-case)
   - Update `authors` with your information
   - Modify `requires-python` if needed
   - Update dependencies as required
   - Change the `[project.scripts]` entry point name

4. **Rename the package directory**:
   - Rename `src/python_template/` to `src/your_package_name/` (use snake_case)
   - Update all imports throughout the codebase
   - Update the `.gitignore` file to reference your new package name instead of `python_template`

5. **Update test files**:
   - Review and modify tests in `tests/` directory for your use case
   - Update imports in test files to use your new package name
   - Add or remove test files as needed for your project

6. **Update the README**:
   - Replace the title and description
   - Update command examples with your new package name
   - Remove or customize this Template Setup section

7. **Initialize your environment**:
   ```bash
   uv sync --dev
   ```

8. **Verify everything works**:
   ```bash
   uv run pytest
   uv run ruff check
   uv run ty check
   ```

9. **Commit your changes** and start building!
