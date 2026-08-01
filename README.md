# Imprint Plays

10 games that run inside [Imprint](https://imprint.selfactual.ai) — or any Claude instance with these gears loaded.

Not personality quizzes. Not therapy. The point is the weird moment where something real comes out of something that felt like a game.

**Chaos goblin energy with a vault underneath.**

---

## Invoke

In any Imprint session, say one of:

- `imprint plays`
- `let's play`
- `game time`
- `play something`

Imprint loads the game menu and you pick from there.

---

## The 10 games

| # | Game | What it is |
|---|------|------------|
| 1 | Word Association | Back and forth words — Imprint reacts to the weird ones |
| 2 | Two Truths & a Lie | You give 3, Imprint guesses the lie using your vault |
| 3 | Would You Rather | Imprint picks tough either/ors from your actual life context |
| 4 | Rank These | 5 things, you rank them, the order tells a story |
| 5 | Am I The Asshole? | Imprint presents an ambiguous scenario, you judge it |
| 6 | Desert Island | 5 items, you pick 3, you explain why — the why is the game |
| 7 | Story Chain | One sentence each, back and forth, no plan |
| 8 | Guess What Imprint Thinks | Imprint makes a confident (often wrong) guess about you |
| 9 | Young [Name] | Imprint describes a scenario for you at age 8–12, you answer as that kid |
| 10 | Mad Libs | Collaborative chaos — Imprint fills a template using your vault |

---

## How it works

The `imprint-games` wrapper gear loads the manifest (`imprint-plays-manifest`), which indexes the 10 game slugs. Imprint reads each game doc from your personal vault on demand.

**With SelfActual + Imprint:** Full vault-powered play. Profile loaded = weirdly specific guesses. The chaos goblin knows you.

**With generic Claude:** Paste the gear `.md` files into your context (or upload them). No vault = pure chaos mode. Still works — thin profile is more fun, not less.

---

## Files in this repo

```
gears/
  imprint-games.md           ← wrapper gear (loads manifest + menu)
  imprint-plays-manifest.md  ← index of all 10 game slugs
  plays-word-association.md
  plays-two-truths.md
  plays-would-you-rather.md
  plays-rank-these.md
  plays-aita.md
  plays-desert-island.md
  plays-story-chain.md
  plays-guess-imprint-thinks.md
  plays-young-name.md
  plays-mad-libs.md
```

---

## Install

**SelfActual users:** download [`gears/imprint-plays-installer.md`](gears/imprint-plays-installer.md), paste it into Imprint, say "install imprint plays." All 13 vault documents created automatically.

**Generic Claude:** paste [`gears/imprint-games.md`](gears/imprint-games.md) into any Claude conversation and say "imprint plays." No vault needed — runs in pure chaos mode.

See [INSTALL.md](INSTALL.md) for details.

## Testing & feedback

See [TESTING.md](TESTING.md) for what to look for and how to give feedback.

---

*Built by Jay + Imprint across one very chaotic session. Blame Brad for approving it.*
