---
description: Set up Transcript to Blog. Connects Google Drive and lets you choose your transcript folder (source) and your blog folder (destination). Run this once after installing.
---

Run the transcript-to-blog first-run setup as a warm, guided wizard. Run it even if some configuration already exists, because the user may be reconfiguring their folders.

Follow the "First-run setup" steps in the transcript-to-blog skill:

1. Connect Google Drive. Surface the connect action directly in the thread so it is one click. Only fall back to a friendly one-line pointer if you cannot surface it. Wait until Drive is connected before continuing.
2. Ask which Drive folder her transcripts live in (the source folder). Confirm by listing a file or two from it.
3. Ask which folder the finished blogs should be saved to (the destination folder).
4. Ask if she wants a file-naming convention. If not, default to the blog title plus the date.
5. Save the config to your memory and to a `transcript-to-blog-config.json` file in the destination folder, so setup never has to run again unless she changes something.

Do the work for her, do not hand her instructions. Only ask when you genuinely need her input. Always carry a friendly fallback so nothing ever dead-ends. Confirm in one line when setup is complete, and tell her she can now blog a transcript any time.
