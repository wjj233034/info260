# Usability Testing Evidence

## Purpose and method

Two participants reviewed the initial V1 prototypes for **My Appointment** and **My Profile**. Each participant followed the same task-based test: identify key appointment details, change an appointment, cancel an appointment, locate preparation guidance, update profile information, discard an edit and change reminder preferences. Follow-up questions explored clarity, missing information and the most important improvement.

Participant 1 interacted with the working prototype and reported task outcomes and interface reactions. Participant 2 completed a structured walkthrough using the uploaded HTML controls and implemented interaction logic. Because Participant 2 could not run the local `file://` pages as a complete desktop Chrome or Safari session, their comments are treated as task-flow feedback rather than direct observation of full browser rendering.

Raw responses were consolidated and paraphrased below to produce a consistent report format. No additional participant claims were invented.

## Participant 1 findings

### Task completion

| Task | Outcome | Observation |
| --- | --- | --- |
| Locate doctor, date, time and fee | Completed | The participant found the key details immediately in the upcoming-appointment card. |
| Change the appointment | Completed | The selected date and time were updated and a confirmation message appeared. |
| Cancel the appointment | Completed | The confirmation dialog clearly separated keeping and cancelling the appointment. |
| Locate preparation guidance | Completed | The preparation checklist was easy to identify in the supporting panel. |
| Update phone and pharmacy | Completed | Both changes saved successfully and were reflected on the page. |
| Discard profile edits | Completed | The original information was restored and the system confirmed that changes were discarded. |
| Disable appointment reminders | Completed | The switch responded immediately and provided status feedback. |

### Main observations

- Appointment details had a clear visual hierarchy and were easy to scan.
- The expanded change-time area lacked an obvious way to leave without making a change, particularly on a narrow screen.
- A generic confirmation label did not clearly communicate that it would confirm a new appointment time.
- The cancellation step did not explain deadlines, charges or refund consequences.
- The profile edit control was less prominent than the information it controlled.
- The emergency-contact name and telephone number would be easier to maintain as separate fields.
- Confirmation dialogs and notification switches were considered the simplest interactions.

### Priority recommendation

Participant 1 prioritised clearer cancellation consequences because the decision can affect both the appointment and the consultation fee.

## Participant 2 findings

### Task completion

| Task | Outcome | Observation |
| --- | --- | --- |
| Locate appointment details | Completed | Doctor, date, time, consultation type and fee were grouped effectively. |
| Change the appointment | Completed | The task was possible, although the controls only became visible after activating the change action. |
| Cancel the appointment | Completed | The two-stage confirmation made the consequence understandable. |
| Locate preparation guidance | Completed | The checklist was clearly separated from the main appointment information. |
| Update personal and healthcare details | Completed | The separate editing areas supported both save and discard actions. |
| Disable appointment reminders | Completed | This was considered the most direct task because the control was immediately actionable. |

### Main observations

- The change-appointment path was the least discoverable part of the prototype because its date and time controls were initially hidden.
- The term **Confirm** needed more context about the action being completed.
- Cancellation and rescheduling needed information about deadlines, fees and refunds.
- Profile editing, restoration of discarded values and reminder controls formed a complete and understandable task flow.
- Participant 2 suggested using plain action-oriented wording such as **Change Date & Time** and **Confirm New Appointment**.

### Overall assessment

Participant 2 rated My Appointment 8/10 and My Profile 9/10. The profile scored more strongly because its edit, save, discard and notification behaviours were internally consistent. The appointment page remained usable, but the change-time action required clearer signposting.

## Consolidated analysis

The two participants completed every assigned task. Both identified the same three improvement themes:

1. Make the change-date-and-time path more visible and easier to leave safely.
2. Replace generic confirmation wording with labels that state the exact action.
3. Explain cancellation and rescheduling consequences before the user commits.

They also agreed that the appointment summary, preparation guidance and profile reminder controls were strong parts of the design. This convergence made the appointment-change flow and policy information the highest-priority iteration areas.

## Design response

| Consolidated finding | Implemented response |
| --- | --- |
| Change-time controls were initially hidden and could fall below the viewport. | Renamed the entry action **Change Date & Time**, moved focus into the opened area and automatically scrolled it into view. |
| The user needed an explicit way to leave the change flow. | Added **Keep Current Appointment** and Escape-key behaviour. |
| The confirmation label lacked context. | Renamed it **Confirm New Appointment**. |
| Cancellation and rescheduling consequences were absent. | Added a visible policy covering the deadline, fee and refund consequence, plus confirmation that the consultation fee remains unchanged after rescheduling. |
| Profile edit and discard actions needed clearer scope. | Used section-specific edit/save labels and renamed the exit action **Discard Changes**. |
| Emergency-contact data was combined. | Separated contact name and telephone number. |
| Some profile inputs could accept unreliable values. | Added telephone validation, a pharmacy selection list and protection for identity fields. |
| Notification controls behaved differently from edited sections. | Added a note explaining that notification switches save automatically. |

## Evidence status and limitation

Both participants evaluated V1, so their feedback provides a strong combined basis for the revisions, but it does not by itself demonstrate that a participant validated the revised version. For stronger iteration evidence, a participant should complete a short follow-up test on Iteration 2. Screenshots should show V1, the consolidated findings and the corresponding Iteration 1/Iteration 2 changes without claiming that Participant 2 used a complete desktop-browser environment.
