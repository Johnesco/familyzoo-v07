# Family Zoo — v07 — Locked Doors & Keys

A staff gate now blocks passage south until the player finds the keycard at the entrance and unlocks it. Covers the full locked-door stack: keys, LockableTrait, DoorTrait, and the via property on exits.

Step 7 of the [Family Zoo](https://github.com/Johnesco/familyzoo) tutorial — a progressive walkthrough of the [Sharpee](https://sharpee.net) TypeScript interactive fiction engine, from a single room to a full multi-file story.

## What this step teaches

- LockableTrait with keyId wiring a specific key to a specific lock
- DoorTrait bridging two rooms bidirectionally
- Exit via property so going checks the door state
- The take, unlock, open, go player sequence
- Ordinary items serving as keys — no special trait needed

## Playing

Open `play.html`, or preview the folder:

```bash
python -m http.server 8000 --directory familyzoo-v07
```

## Building

This is a **frozen 0.9.x TypeScript version**. The built player in this folder is the published artifact; it is re-laid from `browser/` by the workspace build:

```bash
python ../tools/build.py familyzoo-v07
python C:/code/ifhub/tools/ship.py familyzoo-v07
```

The authoring tree for every version lives in the [familyzoo](https://github.com/Johnesco/familyzoo) repo.
