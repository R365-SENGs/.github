# R365 Automations Team - Operational Documentation

## Toolset Standards 

### Python

*_Minimum Python Version >=3.11_*
1. Linting/Formatting - [Black](https://black.readthedocs.io/en/stable/index.html)
2. Dependency Management - [Poetry](https://python-poetry.org/)
3. Testing - [pytest](https://docs.pytest.org/en/stable/)

### Preferred Python Modules 
  * Data Processing (Conditionals) - [numpy](https://numpy.org/doc/stable/)
  * Data Processing (General) - [pandas](https://pandas.pydata.org/docs/)
  * Data Modeling - [pydantic](https://docs.pydantic.dev/latest/)
  * HTTP Handling - [requests](https://pypi.org/project/requests/)

### General Recommendations
  * Notes - [Obsidian](https://obsidian.md/)

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


## Contribution Standards

### Production-Targeted Development Checklist
_In this context, production-targeted means work on a scoped project that was added by external client request._ 
_Requests from clients internal to R365 (SENG leadership, CS, product teams) should have their projects managed in separate modules._
_Production-targeted functionality should be managed via the steps below._
1. Open an issue in the repository describing the bug fix or feature request.
2. If you intend to address the request, assign yourself to the issue for tracking purposes.
3. Clone the *_main_* branch of the repository into a local environment.
4. Create a new branch, preferably with the same name as your open issue.
5. Before submitting a merge request, review the following:
      * Check for hardcoded data.
      * Incorporate clear docstrings for all functions. +1 if you include parameter descriptions.
      * Run Black for linting/formatting.
      * Create or update the pyproject.toml via Poetry for dependency management.
      * Create or update .gitignore to screen any customer or authentication data out of the commit.
      * Add or update a relevant section of the README.md
      * Ideally, add unit or output tests for standalone modules, integration testing for bug fixes. Do tests pass at 80%+?
6. Commit and push! 
