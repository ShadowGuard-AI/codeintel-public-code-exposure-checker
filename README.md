![Banner](banner.png)

# codeintel-Public-Code-Exposure-Checker
Identifies code snippets and sensitive data (API keys, database credentials, internal IP addresses) accidentally exposed on public websites or repositories. The search itself is simulated: the program analyses a fixed set of example results, it does not call a search engine API, so the findings are the same whatever search term is given. Focused on tools for static code analysis, vulnerability scanning, and code quality assurance.

## Install
`git clone https://github.com/ShadowGuard-AI/codeintel-public-code-exposure-checker`

## Usage
`python3 main.py SEARCH_TERM [-o OUTPUT] [-v]`

## Parameters
- `-h`: Show help message and exit
- `search_term`: The search term to use (for example 'API_KEY in:github'). Use Google Dorks.
- `-o`, `--output`: Output file to save results (optional).
- `-v`, `--verbose`: Enable verbose logging (debug level).

## Verified behavior
- Running with a search term prints the simulated findings (example API keys, a database credential, and example IP addresses) and exits 0. Do not treat these example findings as results for the search term given.

## License
See LICENSE.
