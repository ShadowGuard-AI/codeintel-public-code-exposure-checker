![The carvers yard before any name is given: the finished figurehead on her trestles where the low harbour light lands first, a half finished lion and a half finished eagle on their own trestles, mallets and chisels resting on the bench between them, tarred barrels by the shed door, timber baulks leaning in a stack, and the flat harbour beyond the fence, with no lettering anywhere](intro-banner.png)

# codeintel-public-code-exposure-checker

Title block: the name above is set in Berkshire Swash on a sail cream plate ruled as a ledger page, with a rope knot at the left of the heading and the carved figurehead mark below. The carved figurehead image appears at major sections; minor sections take plain ruled headings.

![One carved figurehead in plain silhouette in harbour blue: a woman in wood leaning forward at the waist, her hair cut in waves, one arm raised, standing on rope tan trestles on a sail cream ground, with rust red marking only the crack in the timber at her shoulder, and the name hand lettered below in cut strokes](logo.png)

![The yard in working hours: the shed open at the front with its name board carrying the name, a half finished lion on trestles to the left, a half finished eagle to the right, the finished woman between them and largest in the frame, mallets and chisels in a row on the bench, pale shavings on the floor, tarred barrels by the door, unlit oil lanterns on the beams, and paint pots holding white, black, and rust red](banner.png)

![The yard in three depths: light shifting slowly on the flat harbour far away, a lantern flame flickering inside its glass and a mallet lifted from the bench and set down again in a new place in the middle depth, and a curl of shaving dropping from the bench edge and landing once on the floor near](scene.svg)

# codeintel-Public-Code-Exposure-Checker
Identifies code snippets and sensitive data (API keys, database credentials, internal IP addresses) accidentally exposed on public websites or repositories. The search itself is simulated: the program analyses a fixed set of example results, it does not call a search engine API, so the findings are the same whatever search term is given. Focused on tools for static code analysis, vulnerability scanning, and code quality assurance.

> **Yard notice nailed to the shed wall: the search is simulated.** The programme analyses a fixed set of example results and calls no search engine API. The findings are the same whatever search term is given, and a reader must not treat the printed findings as findings about the term they typed.

![Major separator](sep-heavy.svg)

## Install

`git clone https://github.com/ShadowGuard-AI/codeintel-public-code-exposure-checker`

![Minor separator](sep-light.svg)

## Usage

`python3 main.py SEARCH_TERM [-o OUTPUT] [-v]`

![Major separator](sep-heavy.svg)

## Parameters

- `-h`: Show help message and exit
- `search_term`: The search term to use (for example 'API_KEY in:github'). Use Google Dorks.
- `-o`, `--output`: Output file to save results (optional).
- `-v`, `--verbose`: Enable verbose logging (debug level).

> **Yard notice: no dork reaches a search engine.** The parameter entry above tells the reader to use Google Dorks. That instruction is preserved as printed and flagged here: the programme performs no such search, calls no repository host, and makes no network request of any kind.

![Minor separator](sep-light.svg)

## Verified behavior

- Running with a search term prints the simulated findings (example API keys, a database credential, and example IP addresses) and exits 0. Do not treat these example findings as results for the search term given.

> **Yard notice: a run ends at 0 even when it finds exposure.** Only a failed save or an unexpected error ends a run at 1. The exit code says nothing about what was found.

> **Yard notice: found values enter the log in full.** Found values are written into the log in full, so a log file from a run holds those values and must be handled as a file that holds them. No found value is reproduced in this README.

![Major separator](sep-heavy.svg)

## License

See LICENSE.

> **Yard notice: the licence line stands as printed.** The closing line above, See LICENSE, matches the repository, which holds a LICENSE file carrying the MIT License. The heading of this file reads codeintel-Public-Code-Exposure-Checker, with a capital P and a capital C that the repo name does not carry, and no change of directory step follows the clone line. Those gaps are recorded here, not repaired in the prints.
