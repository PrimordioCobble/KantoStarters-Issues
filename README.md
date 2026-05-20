# KantoStarters - Issue Tracker

This repository is used only for bug reports, compatibility issues, and support requests related to the KantoStarters Minecraft mod.

KantoStarters is a Fabric/Cobblemon utility mod for configurable starter selection, reward choices, fossil choices, dojo rewards, gifts, and map events using normal Minecraft blocks.

The source code is currently private and is not distributed publicly.

## Before opening an issue, please include:

- Minecraft version
- Fabric Loader version
- Fabric API version
- Cobblemon version
- KantoStarters version
- Crash report or latest.log, if applicable
- Steps to reproduce the issue

## For choice setup issues, please also include:

- The related `sessionId`
- The related `choiceId`
- The block coordinates and dimension where the choice is bound
- The command you used, such as:

```mcfunction
/kantostarters set <sessionId> <choiceId>
```

- The relevant part of your `choice_sessions.json`
- Whether the issue happens after running:

```mcfunction
/kantostarters reload
```

## For reward or command issues, please also include:

- The `commands` configured for that choice
- The `itemRewards` configured for that choice, if used
- Any server console errors
- Whether the command works when tested manually in-game

## For starter screen issues, please also include:

- Whether the default Cobblemon starter screen is enabled or disabled
- The current setting used with:

```mcfunction
/kantostarters DefaultPickStarters on
/kantostarters DefaultPickStarters off
```

## For dialogue or language issues, please also include:

- Your selected Minecraft language
- The related dialogue ID
- The relevant part of:
  - `choice_dialog_arrays_en_us.json`
  - `choice_dialog_arrays_pt_br.json`

## Main config folder

KantoStarters creates and uses its configuration files inside:

```txt
config/kantostarters/
```

Main files:

```txt
choice_sessions.json
choice_dialog_arrays_en_us.json
choice_dialog_arrays_pt_br.json
```

## Useful commands

```mcfunction
/kantostarters reload
/kantostarters debug
/kantostarters list
/kantostarters set <sessionId> <choiceId>
/kantostarters unset
/kantostarters open <sessionId> <choiceId>
/kantostarters BlockIfAlreadyHasCobblemon <sessionId> <true|false>
/kantostarters DefaultPickStarters on
/kantostarters DefaultPickStarters off
/kantostarters reset all
/kantostarters reset <sessionId>
```

## Official pages

Downloads, changelogs, and mod information are available on the official CurseForge and Modrinth pages.
