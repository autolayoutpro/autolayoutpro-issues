# AutoLayout PRO — Issue Tracker

Public bug tracker for [AutoLayout PRO](https://autolayoutpro.com/), a Figma-like layout engine for Unity uGUI.

The package source lives in a separate private repository. Use this repo to:

- 🐞 **[Report a bug](https://github.com/autolayoutpro/autolayoutpro-issues/issues/new?template=bug_report.yml)**
- 💡 **[Request a feature](https://github.com/autolayoutpro/autolayoutpro-issues/issues/new?template=feature_request.yml)**
- 🔍 **[Browse open issues](https://github.com/autolayoutpro/autolayoutpro-issues/issues)**

## Fastest way to report a bug — use the AutoLayout component's gear menu

When the bug is in a specific layout, **right-click the AutoLayout component header** in Unity's Inspector (or click the gear / 3-dot menu on the right of the header). Two items are available:

| Menu item | What it does |
|---|---|
| **Report a Bug…** | Opens a new GitHub issue with the YAML of *this component's subtree* pre-filled, plus your AutoLayout PRO version, Unity version, and editor platform. |
| **Copy Layout YAML** | Copies the YAML of this subtree to your clipboard. Use for sharing in chats or pasting into a manually-filed issue. |

Result: a one-click issue with everything we need to reproduce — leaving you to describe the symptom and steps.

### What gets pre-filled

- **AutoLayout PRO version** — from the package config
- **Unity version** — `Application.unityVersion`
- **Platform** — `Editor (macOS / Windows / Linux)`
- **Layout YAML** — serialized dump of the clicked component's subtree

### Clipboard fallback for large layouts

GitHub's issue-form URL is limited to about 8 KB. For deep trees the YAML may not fit, in which case **Report a Bug…** copies the full YAML to your clipboard, opens the issue with a placeholder telling you to paste, and shows a confirmation dialog. Just paste (`Cmd/Ctrl + V`) into the Layout YAML field before submitting.

## Alternative entry points

- **Welcome window** — `Window → AutoLayout PRO → Welcome → Quick Links → Report a Bug`. Picks the current selection or the first AutoLayout root in the active scene if nothing is selected.
- **Manual filing** — file via the [bug-report form](https://github.com/autolayoutpro/autolayoutpro-issues/issues/new?template=bug_report.yml) directly.

## Filing manually

If you can't use the editor (e.g. an exception prevents the Welcome window from opening):

1. Check the [docs](https://autolayoutpro.com/) — most usage questions are answered there.
2. Search [existing issues](https://github.com/autolayoutpro/autolayoutpro-issues/issues?q=is%3Aissue) — your bug may already be tracked.
3. Try the latest version — your bug may already be fixed.
4. File via the [bug-report form](https://github.com/autolayoutpro/autolayoutpro-issues/issues/new?template=bug_report.yml).

## What to include

The bug-report form prompts for the essentials. The most useful manual reports include:

- A **minimal reproduction** project or scene (zip up just enough to demonstrate the bug)
- The **exact console output** (Unity's full stack trace, not just the headline)
- **Screenshots or a short clip** of the unexpected behavior
- The **layout YAML** — easiest path is to right-click the AutoLayout component → **Copy Layout YAML**

## Response

This is a one-person operation; bug triage happens in batches. Please be patient — issues with clean repros and the layout YAML attached get prioritised.
