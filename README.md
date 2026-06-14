# SpamTools

A small collection of single page AI tools, each powered by the Gemini API
(gemini-2.5-flash-lite). No backend, no build step, just open the page.

## How it works

Each tool asks for a Gemini API key the first time you open it. The key is
saved in your browser's local storage, so you only enter it once. All tools
share the same stored key. You can update or replace it from the settings
icon inside any tool. Get a free key from
[Google AI Studio](https://aistudio.google.com/app/apikey).

## Structure

```
spamtools/
  index.html          hub page linking to every tool
  spamexcuse.html
  spamroast.html
  spamhoroscope.html
  spamduck.html
  spamhaiku.html
  spamcorporate.html
  spamregex.html
  spamcommit.html
  spamrename.html
  spamsummary.html
  spamprompt.html
```

## Tools

- **SpamExcuse**: describe a situation, get three excuses from mild to absurd.
- **SpamRoast**: paste your code, get roasted, then get one real tip.
- **SpamHoroscope**: enter your stack, get today's reading, a lucky pick, and what to avoid.
- **SpamDuck**: explain your bug, get clarifying questions back, never the answer.
- **SpamHaiku**: describe a code change, get a haiku for the commit log.
- **SpamCorporate**: say what you mean, get the corporate version and a buzzword count.
- **SpamRegex**: describe a pattern in plain English, get the regex for it.
- **SpamCommit**: describe your changes, get a commit subject and body.
- **SpamRename**: describe what something does, get a few naming options.
- **SpamSummary**: paste something long, get a tldr and the key points.
- **SpamPrompt**: paste a rough AI prompt, get a sharper version of it.

## Running locally

Each file is fully self contained. Open it directly in a browser, or serve
the folder with any static file server.

## GitHub Pages

If Pages is enabled for this repo, the hub page and every tool are live at:

```
https://<username>.github.io/spamtools/
https://<username>.github.io/spamtools/spamexcuse.html
```

and so on for each tool file.

## Note on the API key

Since there is no backend, the API key is stored and used directly in the
browser. This is fine for personal use on your own device. Do not share a
page that has your key saved, and do not deploy this somewhere other people
will use with your key.
