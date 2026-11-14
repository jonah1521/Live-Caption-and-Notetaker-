# HANDOFF

**Goal:** Accessible live captioning and note-taking web app for deaf and hard-of-hearing students.

**Live link and repo:** None yet (local setup)

**Files:**
- `index.html` - Main HTML layout for captions and notes
- `README.md` - Project description and user guide
- `HANDOFF.md` - Current state of the project
- `2_scripts/1_data.js` - Speech Recognition state management
- `2_scripts/2_rules.js` - Business rules for handling transcripts and notes
- `2_scripts/3_display.js` - UI updates and DOM manipulation
- `2_scripts/4_start.js` - Application initialization and event wiring
- `3_styles/style.css` - Responsive styles for layout and accessibility

**Working now:** Initial visual interface, speech recognition start/stop, live transcript rendering, side-by-side note editor, copy captions to notes.

**Last session:** Created initial file layout and working core features.

**Next step:** Create GitHub repository, commit initial files, and test locally in Chrome.

**Decisions:** Use browser-native Web Speech API (`webkitSpeechRecognition`) to avoid external API keys or server costs.

**APIs and data:** Web Speech API (`SpeechRecognition` / `webkitSpeechRecognition`), browser-native JavaScript API.

**How to check it:** Open `index.html` in Google Chrome, click "Start Captions", speak into the microphone, and verify live text output.