# Prompt log

## 2026-11-19

- **Asked:** Set up the project folders for a single-file web app, keep `AGENTS.md`, `spec.md`, `prompts.md`, and `index.html` at the root, add folder READMEs, and document the layout and file-placement rule in `AGENTS.md`.
- **Changed:** Created the root placeholders and the four numbered folders with README files; documented the layout and placement rule in `AGENTS.md`.
- **Worked:** Yes; the requested scaffold is in place.

- **Asked:** Review `spec.md` and provide engineering, product, and implementation recommendations without writing code.
- **Changed:** No app code or specification changes were made; reviewed the current scope and identified gaps and recommendations.
- **Worked:** Yes; a prioritized review was prepared, including real beam properties, load/support details, pass/fail criteria, units, validation, and diagrams.

- **Asked:** Update the beam application specification with the reviewed improvements.
- **Changed:** Expanded `spec.md` with real steel/lumber property requirements, imperial units, calculation assumptions, utilization and pass/fail outputs, validation cases, interface expectations, and explicit MVP exclusions.
- **Worked:** Yes; the requested specification update is complete.

- **Asked:** Build the beam section-property database.
- **Changed:** Added `01_data/beam_sections.json` with 11 steel W-shapes and 6 Douglas Fir-Larch lumber sizes, source metadata, units, elastic properties, and preliminary allowable bending values. Updated the data README.
- **Worked:** Yes; the database file is valid JSON and is documented for the static single-file app.

- **Asked:** Build the beam calculator app.
- **Changed:** Replaced the HTML placeholder with a responsive single-file interface and beam-calculation engine in `index.html`, connected it to the JSON section database, and added validation-case documentation.
- **Worked:** The app implements support selection, point and uniform loads, steel/lumber sections, reactions, diagrams, bending, deflection, and Pass/Fail summaries. Run it through a local HTTP server for database loading.

- **Asked:** Fix app startup and load-removal behavior found during browser testing.
- **Changed:** Made the startup example the 20 ft W12x26 uniform-load baseline and reran analysis when point or uniform load rows are added or removed.
- **Worked:** Browser reload confirmed the corrected startup example: 50 kip-ft moment, 0.609 in deflection, 10 kip reactions, and Pass/Pass status.

- **Asked:** Hand-check the validation cases and compare them with the app.
- **Changed:** Found and corrected the cantilever bending-moment sign convention before completing the validation matrix.
- **Worked:** Validation testing is in progress.

- **Asked:** Add a dark mode slider.
- **Changed:** Added a persisted header theme switch and dark-mode CSS variables for the app shell, panels, inputs, and controls.
- **Worked:** Browser verification confirmed the switch enables dark mode and remains selected after reload.

- **Asked:** Add beam section comparison.
- **Changed:** Added a section-comparison table with bending stress, deflection, utilization, Pass/Fail sorting, selected-row highlighting, and selectable result rows.
- **Worked:** Browser verification confirmed the comparison table renders, sorts passing sections by weight, identifies W14x22 as the baseline best pass, and updates the selected section when a row is activated.

- **Asked:** Make the beam-size selector font smaller so its text fits.
- **Changed:** Reduced only the section selector font size to 12px.
- **Worked:** Change applied; browser reload verification pending.

- **Asked:** Explain how to open the app preview.
- **Changed:** No app files changed; provided the local preview URL and server-start instructions.
- **Worked:** Instructions provided.

- **Asked:** Match the orientation selector font size to the shape/size selector.
- **Changed:** Applied the same 12px font size to both selectors.
- **Worked:** Styling change applied and verified in the served HTML.

- **Asked:** Add a summary section that saves the last five tests run.
- **Changed:** Added a recent-tests panel persisted in browser local storage. The Analyze beam button records up to five runs; each entry shows beam section, support, span, outcome, moment, and deflection, with a Load button to restore the saved inputs.
- **Worked:** Browser verification confirmed edits do not create history entries, explicit analyses are saved, only the newest five remain, history survives reload, and Load restores the saved support, material, section, orientation, span, and loads.

- **Asked:** Suggest another feature to add.
- **Changed:** No app files changed; recommended save/load beam scenarios.
- **Worked:** Feature recommendation prepared.

- **Asked:** Suggest another useful app feature.
- **Changed:** No app files changed; recommended the next feature and a few alternatives.
- **Worked:** Feature recommendation prepared.

- **Asked:** Identify what the shown `index.html` screenshot represents.
- **Changed:** No files changed.
- **Worked:** Confirmed the screenshot shows the empty HTML shell, not the completed app or database-driven interface.
