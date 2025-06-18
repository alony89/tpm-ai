# tpm-ai
Ai powered technical program manager

Dev Instructions – Web App

Layout:

Create a web app with a two-panel grid layout occupying 80% of the page width.
  Left panel: Google Calendar integration.
  Right panel: Meeting notes editor.

Left Panel – Calendar Integration:
  Connect to Google Calendar via API or OAuth.
  List today’s meetings (add a dummy meeting if none exist).
  On clicking a meeting, expand it inline to show:
    Attendees grouped by status: Accepted / Declined / No Response
    Meeting description

Right Panel – Notes Template:
  Display a pre-filled note template titled “Internal Meeting” with the following sections:
    Template Name: Internal Meeting
    Meeting Title
    Greeting
    Agenda
    Topic 1
    Topic 2
    Decisions
    Action Items

LLM Integration:
  On right-clicking a meeting in the left panel, show an option: “Create notes”.
  When clicked:
    Send meeting details + template + prompt to LLM:
      “Populate the meeting title based on the meeting details.”
    Display the updated note in the right panel.

Storage:
  Allow user to edit and add notes in the right panel.
  Save the note to a local folder, which the app auto-creates on first use.

