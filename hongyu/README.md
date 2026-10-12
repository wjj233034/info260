# Hongyu Deng Page Handoff

**Owner:** Hongyu Deng  
**Contact:** hde55@uclive.ac.nz  
**Last updated:** 12 October 2026

## Current pages

- `my-appointment.html`
- `my-profile.html`

Open either file directly in a current browser. Both pages are self-contained and the account link moves between them.

## Supporting material

- `site-map.md` contains the current site hierarchy draft.
- `evidence/` contains the reformatted findings from two human participants, the validation record and comparison screenshots.
- `iterations/` preserves V1 and Iteration 1 HTML files for the report.

## Integration notes

- These pages currently use embedded CSS and JavaScript so they remain independently testable.
- The group pages currently use the Kōwhai Health name and a shared stylesheet. The integration owner should align the branding, navigation, typography and colour system before the final submission.
- The remaining global navigation destinations should be connected only after the group filenames are confirmed.
- The cancellation rule is retained as a prototype assumption.
- Pharmacy names, appointment dates and appointment times are example data.
- Authentication, persistent storage, payment and live video services are outside the scope of these medium-fidelity pages.

## Behaviour to preserve during integration

- Change Date and Time panel, focus and exit behaviour
- Cancellation confirmation and cancelled state
- Telephone and email validation
- Save and discard behaviour in both profile sections
- Automatic notification-switch feedback
- Responsive single-column layout on narrow screens

## Recommended repository location

Keep this complete folder at `/hongyu/` in the group repository. Do not overwrite files inside another contributor's directory.
