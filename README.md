# Rewrite for Outlook

Rewrite email text into professional business language using Claude, GPT, Gemini, Grok or Llama — in classic (desktop) Outlook, Mac Outlook, Outlook on the web, or new Outlook for Windows.

## Download

Grab the latest `Rewrite_v1.3.8.0.zip` from the [Releases](../../releases) page and unzip it. Inside:

- **Windows-Classic-Outlook/** — classic (desktop) Outlook. Run `setup.exe`.
- **Mac-Web-NewOutlook/** — Mac Outlook, Outlook on the web, or new Outlook for Windows. See the `INSTALL.txt` inside.

Not sure which you have? Classic Outlook has a traditional File/Home/Send-Receive ribbon and runs as a desktop app you launch from the Start Menu. New Outlook, Outlook on the web, and Outlook on Mac all use the simplified, web-style interface (new Outlook for Windows also shows a "Try the new Outlook" toggle).

If your Microsoft 365/work account supports "Add a custom add-in → Add from URL" (not every account does — personal accounts usually need "Add from File" instead), use this URL directly, no download needed:
`https://smartpac77.github.io/outlook-rewrite-web-pages/manifest.xml`

If you'd rather use "Add from File" without unzipping the full release, [`outlook-rewrite-manifest.xml`](outlook-rewrite-manifest.xml) in this repo is the same file on its own.

## How to use

**Classic Outlook:** select text in an email (or just place your cursor in a paragraph), right-click → **Rewrite**, or click the Rewrite button on the ribbon. The text is replaced in place. Press Ctrl+Z to undo.

**Mac / web / new Outlook:** select text (or leave nothing selected to rewrite the whole message), click the **Rewrite** button in the ribbon to open the task pane, then click one of the **Rewrite → [Language]** buttons.

First time, open Settings to choose an AI provider, paste your own API key, and set your target language(s).

## Known limitation (Microsoft bug)

New Outlook for Windows and Outlook on the web (outlook.live.com — they share the same underlying engine) don't currently support reading only a text selection, even though Outlook itself reports that they do. This is a confirmed Microsoft platform bug, not something this add-in can work around.

Until Microsoft fixes it, Rewrite always rewrites the whole message on those two platforms — the add-in automatically leaves your signature, "Sent from..." tagline, and any quoted/forwarded email below it untouched, so only your own typed reply gets rewritten. **As soon as Microsoft fixes this bug, we'll update Rewrite right away so it goes back to rewriting only the text you select.**

If this is inconvenient in the meantime, use the **classic (desktop) Outlook** version instead — it doesn't have this bug, and it edits or translates exactly the sentence(s) you select.

## Pricing

Try it free for 90 days. After that, a lifetime license is just **$1** — one-time payment, no subscription — [buy here](https://payhip.com/b/bGyCq). 30-day money-back guarantee.

All proceeds are donated to charities supporting orphans and underprivileged students in Ethiopia and Tanzania.

## Requirements

Your own API key from any supported provider (most offer free trial credit), plus one of:

- Windows with classic (desktop) Outlook (Microsoft 365 or Office)
- Mac Outlook, Outlook on the web, or new Outlook for Windows
