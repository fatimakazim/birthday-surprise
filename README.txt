BIRTHDAY CARD — SINGLE-FILE VERSION

Files:
- index.html: the complete website (HTML, CSS and JavaScript are embedded)
- assets/song.mp3: the soundtrack used by the music player

Flow (7 stages, strictly in order):
1. Envelope        - tap the seal
2. Card + music    - "see our album"
3. Photo album     - look through all 3 memories to unlock the next step
4. Five notes      - read all 5 handwritten notes, one at a time
5. Three wishes    - pick all 3 flowers to unlock the next step
6. Finale
7. Personal letter - "back", or "start from the beginning" to replay

Navigation:
- Primary pill button (rose, "label →") always moves forward.
- Quiet pill button ("← back") moves to the previous stage; inside the notes it steps to the previous note.
- A thin rose line at the top of the page shows overall progress.
- A small ♪ button (top-right, from the album onward) pauses / resumes the song.
- Browser Back / Forward and the left / right arrow keys also work. Stages that are not finished yet cannot be skipped.

Preview:
1. Keep the assets folder next to index.html.
2. Open index.html in a modern browser.

Customize:
- Open index.html in a text editor.
- Near the start of the script, edit the C object to change names, messages, captions, notes and wishes.
  (C.notes.items holds the five handwritten notes - replace them with your own.)
- Replace assets/song.mp3 with your own MP3, keeping the same filename. The song loops during the whole experience.
- To add real photos, edit the album section in the script and use image elements with files placed in an assets folder.

Deploy:
- Netlify: drag the folder containing index.html and assets/ into Netlify Drop.
- GitHub Pages: upload index.html and assets/ to the root of a repository, then enable Pages for the main branch/root.
- Vercel: import the repository as a static site; no build command is needed and the output directory is the project root.

Notes:
- No React, npm, build tools, or third-party JavaScript dependencies are required.
- The design uses system font fallbacks, so it does not download web fonts.
- Music playback is subject to browser autoplay rules; the envelope tap starts the track where permitted.
- A public deployment URL is accessible to anyone who has the link unless you add hosting-level access protection.
