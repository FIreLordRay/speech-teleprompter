# Speech Teleprompter

A free teleprompter that runs in your browser. Import your speech, set your pace, and present. Nothing to install, no account, no server. Everything is in one file: `index.html`.

## Use it

- **Online:** open the GitHub Pages link for this repo (see *Publish with GitHub Pages* below).
- **Offline:** download `index.html` and double-click it.

1. Click **Edit / import script**.
2. Click **Import file**, drag a file onto the box, or paste your text in.
   - Works with Word (`.docx`), `.txt` and `.md` files.
   - For a Google Doc, use **File → Download → Microsoft Word (.docx)**, or copy and paste the text.
3. Press **Done**, then press **Space** to start. You get a 3-second countdown first.

Your script and settings are saved in your own browser, so the next time you open the page they're still there. Nobody else sees them.

## Delivery marks

Add these to your script to show cues while you read:

| Type this | You see | Means |
|---|---|---|
| `## Opening` | Blue section label | Where you are in the speech |
| `*word*` | Orange word | Lean on this word |
| ` / ` | Green slash | Short breath |
| `[PAUSE]` | Green "pause" tag | Full stop, let it land |
| `==a line==` | Yellow highlight | Say it from memory and look up |
| `[NAME]` | Red tag | Fill this in before you speak |
| `[ANY CUE]` | Green tag | Any stage cue, like `[CLICK TO SLIDE 3]` |

Leave a blank line between paragraphs.

## Controls

| Key | Action |
|---|---|
| Space or click the text | Start / pause |
| ↑ ↓ | Nudge the text up or down |
| ← → | Slower / faster pace (5 words per minute per press) |
| + − | Bigger / smaller text |
| Home | Back to the top |
| E | Edit or import the script |
| M | Mirror the text (for a glass teleprompter) |
| F | Fullscreen |

The pace is in **words per minute**, so the clock at the bottom shows how long the speech runs and how much time is left. Most people speak at 130 to 150 wpm.

The screen stays awake while the speech is scrolling, in browsers that allow it.

## Publish with GitHub Pages

1. On GitHub, go to **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**, pick `main` and `/ (root)`, and click **Save**.
3. After a minute, the page is live at `https://<your-username>.github.io/speech-teleprompter/`.

## How it works

Plain HTML, CSS and JavaScript in a single file. Word files are read in the browser with [mammoth.js](https://github.com/mwilliamson/mammoth.js), loaded from cdnjs. Your files are never uploaded anywhere. Fonts come from Google Fonts. Without internet, everything still works except Word import and the custom fonts.
