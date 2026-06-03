# Transcript to Blog

Turns one of your video transcripts into a finished blog post in your voice, and saves it straight to Google Drive. You give it a transcript, it gives you a blog that needs only a light edit before it goes into Squarespace. It reads the transcript from Drive, so you can do this before the video is even live on YouTube.

## Step 1 — Install it (one time)

The quickest way: paste these three lines into co-work, one at a time.

```
/plugin marketplace add DrDaveHeath/drdaveheath-tools-993cf8
/plugin install transcript-to-blog
/reload-plugins
```

Prefer clicking to typing? Type `/plugin` and open the plugins menu, choose **Add marketplace**, and paste this same line when it asks for the source:

```
DrDaveHeath/drdaveheath-tools-993cf8
```

Then install **Transcript to Blog** from the list. Either route gets you to exactly the same place, so use whichever feels easier.

## Step 2 — Set up your folders (one time)

Type:

```
/blog-setup
```

It runs a short guided setup, about a minute, and asks you three things:

1. To connect your Google Drive, if it is not already connected. One click.
2. Which Drive folder your transcripts live in (the source).
3. Which folder finished blogs should be saved to (the destination).

It remembers all of this, so you only ever do it once. If you move your folders later, just run `/blog-setup` again.

## Everyday use

Once it is set up, just ask in plain language. For example:

- "Blog the latest transcript."
- "Turn this transcript into a blog post." (then paste it)
- `/blog-this`

It picks the right style for the post, writes it in your voice, and saves both a markdown version and a plain-text version to your destination folder. Then it tells you the title and where it saved it.

## A couple of things to know

- It reads the transcript from Google Drive, so it works before your video is live on YouTube. That means you can publish the blog and the video together.
- Squarespace does not allow automatic posting, so the last step (pasting the markdown into Squarespace and publishing) stays manual, the same as now.
- It only ever adds new files. It never changes or deletes anything you already have.

## Questions or changes

If you want it to behave differently, or you change your folders, just tell it, or get in touch with Dave.
