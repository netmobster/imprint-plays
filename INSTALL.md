# Installing Imprint Plays

Two paths depending on your setup.

---

## Option A — SelfActual vault (recommended)

You'll create each gear file as a personal vault document. These stay in YOUR vault — they don't touch any shared product pod.

### What you need

- A SelfActual account with an active Imprint session
- The `create_document` tool available via the SelfActual MCP connector

### Steps

For each `.md` file in `gears/`, run `create_document` with:

```
username:  your-vault-username
slug:      [filename without .md — e.g. "imprint-games"]
title:     [from the frontmatter title field]
content:   [full file content, including frontmatter]
docType:   "reference"
tags:      ["imprint-plays", "gear", "game"]   ← or "wrapper" / "manifest" as appropriate
```

**Install order matters:** install the 10 game gears first, then the manifest, then the wrapper.

```
1. plays-word-association
2. plays-two-truths
3. plays-would-you-rather
4. plays-rank-these
5. plays-aita
6. plays-desert-island
7. plays-story-chain
8. plays-guess-imprint-thinks
9. plays-young-name
10. plays-mad-libs
11. imprint-plays-manifest
12. imprint-games
```

### Verify

Open a new Imprint session and say `imprint plays`. You should see the menu with all 10 games.

---

## Option B — Generic Claude (no SelfActual account)

Paste the gear files directly into Claude's context. No vault, no setup, no slugs.

### Steps

1. Start a Claude conversation
2. Paste the contents of `gears/imprint-games.md` as your first message
3. Paste in whichever individual game gears you want available
4. Say `imprint plays` or `let's play`

### What to expect

Without a vault profile, Imprint runs in **pure chaos mode** — guesses are unhinged, associations are wilder. Two Truths & a Lie won't have vault reasoning to draw on. Guess What Imprint Thinks becomes a confident fever dream.

Thin profile = more fun, not less. Try it.

---

## Updating a gear

If a gear gets updated, re-run `create_document` with the new content. The slug stays the same — it replaces in place.

Or if you're using the generic Claude path: just paste the updated `.md` file.

---

## Removing a game

Delete the vault document with `delete_document` using the slug. Update `imprint-plays-manifest` to remove it from the active list.

Don't delete retired games from the manifest — they live in the Retired table for reference.
