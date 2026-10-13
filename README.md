# TK Mythic+ Count: issues and feedback

Public issue tracker for **TK Mythic+ Count**, a World of Warcraft (Retail,
Midnight) addon for Mythic+: enemy forces per mob, a current-pull readout
stacked on a progress bar, milestone markers, and a keystone timer.

This repository holds no source code. It exists so bug reports and suggestions
have one place to live.

- **Game version:** WoW 12.1.5 (Interface `120105`).
- **Current release:** 1.0.1. The [changelog](https://www.curseforge.com/projects/1740033)
  is on the CurseForge project's Files tab.

## Install

Get the addon from [CurseForge](https://www.curseforge.com/projects/1740033), or
unzip it into `World of Warcraft/_retail_/Interface/AddOns/` so the folder is
`AddOns/TKMythicPlusCount`. Then reload the game.

## Using it

- `/tkmpc` opens the settings window, with a tab per feature.
- `/tkmpc unlock` / `lock` lets you drag the progress bar; the small Lock /
  Unlock button on the bar does the same.
- `/tkmpc timer on` enables the keystone timer panel (off by default).
- `/tkmpc test pull` previews the bar with a fake pull.
- `/tkmpc profile <name>` switches profile. Profiles can be per character or per
  specialization, and exported or imported as a short string.
- `/tkmpc help` lists every command.

Things worth knowing:

- The game hides each living enemy's value from addons during a key, so the
  current pull is drawn as stacked blocks on the bar. "+X% this pull" under the
  bar counts what you have killed since the pull began.
- Milestone percentages marked `~` are not verified yet. You can set your own on
  the Milestones tab.

## Posting an issue

1. [Search the existing issues](../../issues) first; yours may already be there.
2. [Open a new issue](../../issues/new/choose) and pick the matching form.
3. Include, as far as you can:
   - what you expected and what happened instead
   - the dungeon and key level, if it happened in a key
   - your nameplate addon (Blizzard, Platynator, EllesmereUI, Plater, ElvUI, ...)
   - the addon version (shown on the settings window's About tab)
   - your game build (type `/dump GetBuildInfo()` in chat)
   - any Lua error text (an addon such as BugSack makes these easy to copy)
   - a screenshot, if it is a display problem

Please do not paste exported profile strings that contain anything you consider
private.
