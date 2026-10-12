# Iteration 2 Validation

## Validation scope

The revised My Appointment and My Profile pages were checked against the issues identified during the initial usability tests. The validation covered action labels, cancellation information, form validation, healthcare preferences and account-detail controls.

## Confirmed improvements

- The appointment-change entry now uses the clearer label **Change Date & Time**.
- The expanded change area provides **Keep Current Appointment** as an explicit exit action.
- The final change action is labelled **Confirm New Appointment**.
- Cancellation and rescheduling information explains the current two-hour policy assumption and the NZ$45 fee consequence.
- Invalid alphabetic telephone input is rejected and the page remains in edit mode.
- Pharmacy selection uses a controlled list rather than unrestricted text.
- Legal name and date of birth are protected as read-only identity fields.
- Personal-information and healthcare-preference actions use section-specific edit, save and discard labels.
- Emergency-contact name and telephone number are stored as separate fields.

## Issue found during validation and final response

The first clean export had removed the original external icon dependency, leaving empty icon containers. The final handoff replaces those elements with self-contained inline SVG icons. This keeps the pages independent of external libraries while restoring the intended visual cues.

The two completed pages link to one another using relative file links. Other global navigation destinations and account sections belong to the wider group prototype and remain integration tasks; no false or broken destination was added to this individual handoff.

## Validation limitation

The final package has been checked for code structure, link targets, input rules and interaction states. The group should perform one final integrated walkthrough after the shared navigation and stylesheet are applied.
