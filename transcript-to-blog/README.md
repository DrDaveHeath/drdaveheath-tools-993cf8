# Transcript to Blog

Turns one of your video transcripts into a finished blog post in your voice, and saves it straight to Google Drive. You give it a transcript, it gives you a blog that needs only a light edit before it goes into Squarespace.

## Install (one time)

In co-work:

1. Add the plugin source:
   ```
   /plugin marketplace add https://drdaveheath.com/<your-link>
   ```
2. Install it:
   ```
   /plugin install transcript-to-blog
   ```
3. Reload:
   ```
   /reload-plugins
   ```

## First run (one time)

The first time you use it, it will ask you a couple of quick questions:

1. To connect Google Drive, if it is not already connected. One click.
2. Which Drive folder your transcripts live in (the source folder).
3. Which folder finished blogs should be saved to (the destination folder).

It remembers all of this, so you only do it once.

## Everyday use

Just ask, in plain language. For example:

- "Blog the latest transcript."
- "Turn this transcript into a blog post." (then paste it)
- "/blog-this"

It will pick the right style for the post, write it in your voice, and save both a markdown and a plain-text version to your destination folder. Then it tells you the title and where it saved it.

## A couple of things to know

- It reads the transcript from Google Drive, so it works before your video is live on YouTube. That means you can publish the blog and the video together.
- Squarespace does not allow automatic posting, so the last step (pasting the markdown into Squarespace and publishing) stays manual, the same as now.
- It only ever adds new files. It never changes or deletes anything you already have.

## Questions or changes

If you want it to behave differently, or you change your folders, just tell it, or get in touch with Dave.
