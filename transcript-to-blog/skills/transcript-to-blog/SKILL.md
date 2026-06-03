---
description: Turn a video transcript into a finished blog post in Gillian's voice and save it to Google Drive. On first use it runs a short setup (connect Drive, pick the source and destination folders), then runs frictionlessly: transcript in, blog out.
---

# Transcript to Blog

Turn a video transcript into a publish-ready blog post in Gillian Perkins' voice. Read the transcript from one Google Drive folder, write the finished blog to another. On first use, run a short setup. After that, just take a transcript and produce the blog.

She is an experienced content creator, not a beginner. Be warm, brief, and never over-explain.

## How to run this (experience design)
Do the work for her, do not hand her instructions. Whenever co-work can do something natively (surface a "connect" button, open a connector, list folders), trigger that yourself at the right moment rather than telling her where to click. The whole setup should feel like a smooth one-minute wizard that you are running for her. Only ask her a question when you genuinely need her input. Always carry a friendly fallback so it never dead-ends: if you cannot surface an action directly, guide her through it warmly in one line. She should not need to know or care what is native to co-work and what is this plugin. She should just feel that it was easy.

## On every invocation, follow this order

### Step 1 — Load the saved config
Look for the saved configuration: whether Google Drive is connected, the **source folder** (where transcripts live), the **destination folder** (where blogs are saved), and any file-naming convention. Check in this order:
1. Your memory, for the transcript-to-blog config.
2. A file named `transcript-to-blog-config.json` in her Google Drive.

If the config is complete and Drive is connected, go straight to **Normal run**. If anything is missing, run **First-run setup**.

### First-run setup (only when the config is missing)
Open warmly: tell her you will get her set up in about a minute, then run these steps as a guided wizard.
1. **Get Google Drive connected.** Check whether the Google Drive connector is available and authorised. If it is, say so and move on. If it is not, surface the connection for her directly in the thread (trigger the connect action / button) so she can authorise it in one click. Only if you cannot surface it directly, fall back to a single friendly line pointing her to co-work's connector settings. Wait until Drive is connected before continuing.
2. **Source folder.** Ask which Drive folder her transcripts live in. She works pre-publish, so the transcript sits in Drive before the video goes live on YouTube. Confirm by listing a file or two from that folder.
3. **Destination folder.** Ask which folder the finished blogs should be saved to.
4. **Naming convention.** Ask if she wants a file-naming convention. If not, default to the blog title plus the date.
5. **Save the config** to your memory and to a `transcript-to-blog-config.json` file in the destination folder, so setup never runs again unless something changes.
6. Confirm setup is done in one line. If she has already given you a transcript, continue to a normal run.

### Normal run
1. **Get the transcript.** She will either paste it, name a file, or ask for the latest in the source folder. If she says "the latest" or similar, list the source folder and take the most recent transcript file. Only process what she asks for, never auto-process every file in the folder.
2. **Generate the blog.** Load and follow the bundled voice files:
   - `${CLAUDE_PLUGIN_ROOT}/voice/blog-generation-prompt.md` — the operating instructions. Follow them exactly.
   - `${CLAUDE_PLUGIN_ROOT}/voice/brand-voice.md` — the full voice profile, for reference.
   Re-compose from the transcript, do not clean it up. Pick the archetype (personal story, industry commentary, or how-to) from the transcript's content. Write a fresh sensory hook, cut the tangents and side-stories, strip the spoken filler, keep her mechanics (caps, em dashes, ellipses, emoji), and land the emotional double close. Produce both a markdown version and a plain-text version.
3. **Save to Drive.** Write the blog to the destination folder in markdown and plain text, using the naming convention.
4. **Hand it back.** Tell her the blog title, the folder it is saved in, and remind her it is ready for a light edit and paste into Squarespace. (Squarespace cannot be published to automatically, so the paste stays a manual step.)

## Standing rules
- She blogs before the video is published on YouTube, so the transcript always comes from Google Drive, never from YouTube.
- Keep her in control. Only ever add new files. Never delete or overwrite her existing files.
- If she wants to change the source or destination folder later, update the config in both your memory and the Drive config file.
- Never invent statistics, names, or stories that are not in the transcript.
