# v07 — Locked Doors & Keys

A staff gate the player cannot pass until they find the keycard. The refusal message is a named phrase in the en-US catalog, not hardcoded English in the exit.

## What this step adds

- `lockable with the staff keycard`
- `south is blocked while the staff gate is closed: staff-gate-blocked`
- `define phrases en-US` — the catalog of refusal keys
- UNLOCK, LOCK and the messages the stdlib already knows

## The source

The whole step is one file: [`familyzoo-v07.story`](../familyzoo-v07.story). Read it top to bottom — it is the previous step plus what is listed above.

## Running it

```bash
npx sharpee play
npx sharpee test          # replays familyzoo-v07.tests.json
```

Chord language reference: <https://sharpee.net/chord/>
