# Family Zoo — v07: Locked Doors & Keys

A staff gate the player cannot pass until they find the keycard. The refusal message is a named phrase in the en-US catalog, not hardcoded English in the exit.

Step 7 of sixteen in the [Family Zoo](https://github.com/Johnesco/familyzoo) tutorial for [Chord](https://sharpee.net/chord/), the authoring language of the [Sharpee](https://sharpee.net) interactive fiction engine.

## What this step adds

- `lockable with the staff keycard`
- `south is blocked while the staff gate is closed: staff-gate-blocked`
- `define phrases en-US` — the catalog of refusal keys
- UNLOCK, LOCK and the messages the stdlib already knows

## The source

The whole step is one file: [`familyzoo-v07.story`](./familyzoo-v07.story) — the step before it plus the ideas above. The chapter that walks through it is [`docs/v07-locked-doors-keys.md`](./docs/v07-locked-doors-keys.md).

## Playing and testing

```bash
npx sharpee play
npx sharpee test          # replays familyzoo-v07.tests.json
python ../tools/build.py familyzoo-v07 --force
```

## Engine

Pinned to `@sharpee/*` **5.3.0** (Chord 3.6.0), held there by an `overrides` block: 5.3.1 publishes broken subpath exports and breaks `sharpee test`.

The 0.9.x TypeScript edition this replaced is kept in [`legacy/`](./legacy).
