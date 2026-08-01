---
gear: imprint-plays-installer
title: Imprint Plays — Installer
version: 1.0
updated: 2026-08-01
trigger: install imprint plays / install plays
---

# IMPRINT PLAYS — INSTALLER

## What this does

Creates all 13 Imprint Plays vault documents in your personal vault automatically. One command — done.

## How to use

1. Paste this file into an Imprint session (or load it as a document)
2. Say: **"install imprint plays"**
3. Imprint installs all 13 documents to your vault
4. When complete: say **"imprint plays"** to launch the game menu

---

## On trigger: "install imprint plays"

1. Confirm before starting: "Ready to install Imprint Plays — 13 vault documents. Go?" Wait for yes.
2. Get the operator's username from the active vault session.
3. Call `create_document` for each document below, **in the order listed**.
4. After each: report "✓ [slug]" or "✗ [slug] — [plain-language error]".
5. At the end: summary of installed vs failed. If any failed, say which ones to retry.

**Install order:** game gears first (1–10), then manifest (11), then wrapper (12). This order matters — the wrapper loads the manifest, the manifest references the games.

---

## DOCUMENT 1 — plays-word-association

```
slug:    plays-word-association
title:   PLAYS · Word Association
docType: reference
tags:    ["imprint-plays", "gear", "game"]
```

**content:**
```
---
gear: plays-word-association
title: PLAYS · Word Association
version: 1.2
tier: personal
updated: 2026-08-01
category: play
trigger: word association / game 1 / play 1
sourceApp: imprint
---

# PLAYS · WORD ASSOCIATION

## WHAT IT IS
Back and forth. Imprint says a word, operator says the first word that comes to mind. No rules. No wrong answers. The weird ones are the best ones.

## MOVE SEQUENCE

1. Announce: "Word Association. I say a word, you say the first thing that comes to mind. Ready?"
2. Fire a word. Wait. Respond immediately with another word — don't pause to analyze.
3. Keep the chain moving fast. Energy matters more than insight.
4. Run 10 rounds.

## PIT STOP (every 10 rounds)

After 10 words, stop the chain. Pick 2–3 of the most interesting words from the round. React with energy — not clinical analysis. Joke around. Ask about them one at a time.

Tone: two people reacting to a weird thing that just happened — not a debrief, not a therapy session. Banter first.

Then ask: "Keep going or switch games?"

## CALIBRATION SIGNALS
- Speed of response (fast = reflex / slow = considered)
- Emotional temperature of word choices
- What they connect to what (the logic of the leap)
- Words they pause on or take back
- The story behind the weird ones — that's where the chaos goblin lives
```

---

## DOCUMENT 2 — plays-two-truths

```
slug:    plays-two-truths
title:   PLAYS · Two Truths & a Lie
docType: reference
tags:    ["imprint-plays", "gear", "game"]
```

**content:**
```
---
gear: plays-two-truths
title: PLAYS · Two Truths & a Lie
version: 1.1
tier: personal
updated: 2026-08-01
category: play
trigger: two truths / game 2 / play 2
sourceApp: imprint
---

# PLAYS · TWO TRUTHS & A LIE

## WHAT IT IS
User presents 3 statements. Imprint guesses the lie using the vault. Wrong guesses are better than right ones — they invite the real story.

## MOVE SEQUENCE

1. Announce: "Two Truths & a Lie. Give me three statements about yourself. I'll guess which one's the lie."
2. User presents 3 statements. Wait for all three.
3. Imprint uses the vault to reason through which is the lie. Show the reasoning — don't just guess.
4. Commit to a guess. Be wrong sometimes. Wrong is better.
5. User reveals. If Imprint was wrong: "Okay — what's the real story?" The story is the game.
6. Offer another round or switch.

## RULES
- User ALWAYS goes first. Imprint never presents statements about the user — that's a calibration exercise, not a game.
- Show the vault reasoning — "Based on what I know about you, X seems unlikely because..."
- Wrong guesses with good reasoning = great game. Don't hedge to avoid being wrong.

## CALIBRATION SIGNALS
- What they chose to present (what they think is surprising about themselves)
- The lie they chose (what they want to obscure or test)
- How they respond to a wrong guess (defensive? delighted? story-forward?)
- What the truth behind the lie actually is
```

---

## DOCUMENT 3 — plays-would-you-rather

```
slug:    plays-would-you-rather
title:   PLAYS · Would You Rather
docType: reference
tags:    ["imprint-plays", "gear", "game"]
```

**content:**
```
---
gear: plays-would-you-rather
title: PLAYS · Would You Rather
version: 1.0
tier: personal
updated: 2026-08-01
category: play
trigger: would you rather / game 3 / play 3
sourceApp: imprint
---

# PLAYS · WOULD YOU RATHER

## WHAT IT IS
Imprint presents two genuinely difficult choices — drawn from vault context where possible. The choice reveals something. The explanation reveals more.

## MOVE SEQUENCE

1. Announce: "Would You Rather. Two options, you pick one. No 'it depends.'"
2. Present the choice. Make both options uncomfortable in different ways.
3. User picks. Ask: "Why?" — one follow-up only.
4. Imprint says what it would have guessed and why.
5. Run 3–5 rounds. After each, briefly note what the choice revealed without overdoing it.

## RULES FOR GOOD CHOICES
- Both options must be real choices — not obvious
- Use vault context to make them specific: reference real things about the operator's life
- Categories that work well: identity, values, relationships, work, comfort zones
- No gotcha questions. The point is the genuine dilemma, not the trick.

## CALIBRATION SIGNALS
- Speed of decision (fast = clear value / slow = real tension)
- Whether they explain or just pick
- What they optimize for in the explanation
- Where they draw the line
```

---

## DOCUMENT 4 — plays-rank-these

```
slug:    plays-rank-these
title:   PLAYS · Rank These
docType: reference
tags:    ["imprint-plays", "gear", "game"]
```

**content:**
```
---
gear: plays-rank-these
title: PLAYS · Rank These
version: 1.0
tier: personal
updated: 2026-08-01
category: play
trigger: rank these / game 4 / play 4
sourceApp: imprint
---

# PLAYS · RANK THESE

## WHAT IT IS
Imprint presents 5 things. Operator ranks them 1–5. The order tells a story. The explanation tells more.

## MOVE SEQUENCE

1. Announce: "Rank These. I give you 5 things, you rank them 1 to 5. Trust your gut."
2. Present 5 items from a single category. Use vault context to make them specific.
3. User ranks. Ask about the most interesting gap — usually the 1 vs 2 or the 4 vs 5.
4. Imprint reveals what it expected and what surprised it.
5. One follow-up on the most revealing ranking.

## CATEGORIES THAT WORK WELL
- Values (freedom / security / connection / growth / impact)
- Life priorities right now
- Ways you want to be remembered
- Things you're afraid of losing
- Things from a specific life domain (work, relationships, health)

## RULES
- 5 items only. No ties allowed.
- Present as a list, not a question.
- The chaos goblin lives in the gap between expected ranking and actual ranking.

## CALIBRATION SIGNALS
- What goes to #1 (stated priority vs revealed priority)
- What gets buried at #5 (what they're actively moving away from)
- Speed of ranking (fast = clear hierarchy / slow = genuine tension)
- Whether they want to revise after seeing the full list
```

---

## DOCUMENT 5 — plays-aita

```
slug:    plays-aita
title:   PLAYS · Am I The Asshole?
docType: reference
tags:    ["imprint-plays", "gear", "game"]
```

**content:**
```
---
gear: plays-aita
title: PLAYS · Am I The Asshole?
version: 1.0
tier: personal
updated: 2026-08-01
category: play
trigger: am i the asshole / aita / game 5 / play 5
sourceApp: imprint
---

# PLAYS · AM I THE ASSHOLE?

## WHAT IT IS
Imprint presents an ambiguous real-life scenario. Operator judges it. The joke is that you think you're judging a stranger. You're not.

## MOVE SEQUENCE

1. Announce: "Am I The Asshole? I'll describe a situation. You tell me if the person is the asshole or not."
2. Generate a scenario. Rules for good scenarios:
   - Morally ambiguous — both sides have a point
   - Specific enough to feel real (names, settings, details)
   - Vault-calibrated when possible — use contexts the operator knows
   - The setting does work (a Starbucks changes everything)
   - No obvious villains. No obvious heroes.
3. Ask: "Asshole or not? Or somewhere in between?"
4. User gives verdict. Imprint reveals what it predicted and why — using vault reasoning.
5. Dig into the gap between verdict and prediction. That's where the real thing is.

## RULES
- Generate scenarios — no web search, no database
- No Reddit jargon (no YTA/NTA/ESH/NAH). Natural language only: "kind of an asshole," "not the asshole," "both have a point"
- Imprint maps natural language to a verdict internally — never asks the user to learn jargon
- The point isn't the verdict. It's what the verdict reveals about the operator's values.

## CALIBRATION SIGNALS
- How fast they judge (quick = clear values / slow = genuine conflict)
- Whether they see nuance or pick a side hard
- What factors they weight (intent vs impact, context vs rule)
- What makes them defend the "asshole" — that's always interesting
```

---

## DOCUMENT 6 — plays-desert-island

```
slug:    plays-desert-island
title:   PLAYS · Desert Island
docType: reference
tags:    ["imprint-plays", "gear", "game"]
```

**content:**
```
---
gear: plays-desert-island
title: PLAYS · Desert Island
version: 1.0
tier: personal
updated: 2026-08-01
category: play
trigger: desert island / game 6 / play 6
sourceApp: imprint
---

# PLAYS · DESERT ISLAND

## WHAT IT IS
Operator gets 5 items, picks 3 to keep. The why is the game.

## MOVE SEQUENCE

1. Announce: "Desert Island. I give you 5 items. You're stranded — you can only keep 3. Which ones and why?"
2. Present 5 items. Mix practical and symbolic. Use vault context to make at least one personal.
3. User picks 3 and explains.
4. Imprint reacts to the choices — especially the ones dropped and the reasoning behind the keeps.
5. One follow-up on the most surprising choice.
6. Imprint reveals what it predicted they'd pick.

## RULES FOR GOOD ITEM SETS
- Mix categories: practical survival, emotional comfort, creative/intellectual, social/relational
- At least one item with obvious survival value (so dropping it means something)
- At least one item that seems frivolous but might not be
- No obviously correct answers

## CALIBRATION SIGNALS
- What they prioritize (survival vs comfort vs meaning)
- What they drop without hesitation vs what's genuinely hard
- The reasoning — especially when it's unexpected
- What "stranded forever" means to them (do they assume rescue?)
```

---

## DOCUMENT 7 — plays-story-chain

```
slug:    plays-story-chain
title:   PLAYS · Story Chain
docType: reference
tags:    ["imprint-plays", "gear", "game"]
```

**content:**
```
---
gear: plays-story-chain
title: PLAYS · Story Chain
version: 1.0
tier: personal
updated: 2026-08-01
category: play
trigger: story chain / game 7 / play 7
sourceApp: imprint
---

# PLAYS · STORY CHAIN

## WHAT IT IS
We build a story together. One sentence each. You take a turn, Imprint takes a turn. No planning. No knowing where it goes. The choices you make — the direction, the tension, the resolution — reveal more than you think.

## MOVE SEQUENCE

1. Announce: "Story Chain. One sentence each, back and forth. I'll start."
2. Open with a first sentence that has a character, a situation, and just enough ambiguity to go multiple directions:
   Examples:
   - "She opened the drawer she'd never opened before and found something she recognized."
   - "He'd been telling the same story for years, but tonight it finally felt like a lie."
   - "The room was exactly as they'd left it, which was the problem."
   - "They said yes before they knew what they were agreeing to, and it was the best thing that ever happened."
3. User adds their sentence. Imprint adds the next immediately. Keep the energy up.
4. 8–12 turns. End the story when it reaches something that feels complete — don't drag it out.
5. Debrief: "Okay — what did you just tell me about yourself through that story?"
6. If they push back ("nothing, it's just a story"): name what Imprint noticed. Characters they gave agency to. How they resolved tension. What they made important.

## RULES
- ONE SENTENCE per turn. If they write two: "One at a time — don't give me everything 😄"
- Imprint is a generous co-author. Yes-and their direction. Don't block or hijack.
- The story doesn't need to be good. It needs to keep moving.
- Imprint should occasionally introduce pressure — a decision point, a complication — to see how they respond.
- Never interpret out loud during the game. Only after.

## THEMES WORTH STEERING TOWARD
- Agency (who has control in their sentences?)
- Belonging (are characters alone or together?)
- Resolution style (fix it / avoid it / sit with it)
- What they consider an ending vs. what they leave open

## CALIBRATION SIGNALS
- Whether they give characters control or take it away
- How they resolve tension when it's their turn
- What they name as important (objects, relationships, outcomes)
- Whether they went dark or light when they had the choice
```

---

## DOCUMENT 8 — plays-guess-imprint-thinks

```
slug:    plays-guess-imprint-thinks
title:   PLAYS · Guess What Imprint Thinks
docType: reference
tags:    ["imprint-plays", "gear", "game"]
```

**content:**
```
---
gear: plays-guess-imprint-thinks
title: PLAYS · Guess What Imprint Thinks
version: 1.1
tier: personal
updated: 2026-08-01
category: play
trigger: guess what imprint thinks / game 8 / play 8
sourceApp: imprint
---

# PLAYS · GUESS WHAT IMPRINT THINKS

## WHAT IT IS

One unhinged question per round. Imprint makes a confident guess — vault-powered if profile is loaded, pure chaos if it isn't. Wrong answers are better than right ones. The correction is the game.

## FORMAT

### Per round:

1. Ask one absurd, specific question. Good questions are:
   - Specific enough that there's a real answer
   - Weird enough that the answer reveals something
   - NOT therapy ("what's your biggest fear" = out)

   Examples:
   - "What does Imprint think your villain origin story is?"
   - "What does Imprint think you'd do on day one of having $10M?"
   - "What does Imprint think you'd name a boat / band / racehorse?"
   - "What does Imprint think you ordered at a drive-through at 2am last month?"
   - "What does Imprint think your theme song is right now?"
   - "What does Imprint think you were like at 14?"

2. Imprint makes ONE confident guess with reasoning:
   - WITH profile: use vault data in unexpected ways — connect real details to absurd conclusions
   - WITHOUT profile: pure confident chaos — make it up, commit to it
   - Either way: COMMIT. Wrong with confidence beats right with caveats every time.

3. User responds:
   - Agree → "okay that's genuinely unsettling — why do I know that?"
   - Disagree → "okay — what's the real version?" → the story comes out
   - Partial → "what did I get right? what did I miss?"

4. After the response, two paths (light CYOA):
   - "Go deeper on that" → dig into the correction
   - "Next question" → new round

5. After 3 rounds: pick the most interesting gap. "Okay — [specific thing from a correction]. Tell me more."

## TONE

Confident. Slightly wrong. Always curious about the correction. The vault is a tool for building narratives, not reciting facts.

## ON PROFILE

- Loaded: guesses feel weirdly plausible. The moment is "how did you know that?"
- Empty: guesses are pure confident chaos. The moment is the correction.
- Both work. Thin profile = more fun, not less.
```

---

## DOCUMENT 9 — plays-young-name

```
slug:    plays-young-name
title:   PLAYS · Young [Name]
docType: reference
tags:    ["imprint-plays", "gear", "game"]
```

**content:**
```
---
gear: plays-young-name
title: PLAYS · Young [Name]
version: 1.0
tier: personal
updated: 2026-08-01
category: play
trigger: young jay / young name / game 9 / play 9
sourceApp: imprint
---

# PLAYS · YOUNG [NAME]

## WHAT IT IS
Imprint describes a situation for the operator at age 8–12. They answer as that kid — not as who they are now. The kid's response reveals the wiring underneath.

## MOVE SEQUENCE

1. Announce: "Young [Name]. I'll describe a situation for you at [age]. Answer as that kid — not as you now."
2. Use vault context to set the scene. Age 8–12 works best. Be specific — year, season, location if known.
3. Describe the situation. Make it ordinary enough to be real, specific enough to place them there.
4. User answers as their younger self.
5. Imprint reacts — not analytically, with genuine curiosity. "Of course you did." or "Wait — why that?"
6. One follow-up on the most interesting detail.
7. Optionally: "What would [Name] now say to that kid?"

## RULES FOR GOOD SITUATIONS
- Ordinary moments, not big dramatic events
- Situations that involve a choice or reaction, not just a memory
- Use what's known about the operator's childhood from the vault
- Age-appropriate stakes (friend drama, family dynamics, school moments, neighbourhood stuff)

## CALIBRATION SIGNALS
- How quickly they slip into the kid's voice
- What the kid prioritizes (same as adult self? different?)
- How the kid handles conflict, attention, failure, success
- What they remember noticing that adults didn't
```

---

## DOCUMENT 10 — plays-mad-libs

```
slug:    plays-mad-libs
title:   PLAYS · Mad Libs
docType: reference
tags:    ["imprint-plays", "gear", "game"]
```

**content:**
```
---
gear: plays-mad-libs
title: PLAYS · Mad Libs
version: 1.0
tier: personal
updated: 2026-08-01
category: play
trigger: mad libs / game 10 / play 10
sourceApp: imprint
---

# PLAYS · MAD LIBS

## WHAT IT IS
Imprint asks for 5 words/phrases with no context. Then reveals the story they slot into. Snort-worthy by design — the sorbet game. Best played as a palate cleanser between heavier games.

## MOVE SEQUENCE

1. Announce: "Mad Libs. Give me 5 things — no context, just answer fast:"
2. Ask for 5 blanks. Mix categories for best chaos:
   - A place you'd never go back to
   - Something you're weirdly good at
   - A word someone close to you uses that nobody else does
   - Something you own that makes no sense
   - An emotion you don't have a word for
3. User fills in all 5 (can answer all at once).
4. Imprint reveals the story with their answers slotted in. Commit to the bit — play it straight.
5. React to the best one. Ask about it if there's a story there.
6. Offer another round with different blanks or switch games.

## RULES
- Fast answers only. If they overthink: "Don't think. Go."
- The story should be absurd but internally coherent — not random noise
- Use vault context to make the story feel personal where possible
- This is the sorbet game — 5 minutes max, then move on

## CALIBRATION SIGNALS
- What they call "a word nobody else uses" (reveals in-group relationships)
- The "emotion with no name" — often the most revealing blank
- What they own that makes no sense (chaos goblin artifact)
- Whether they want to explain the answers (the ones they explain are the ones that matter)
```

---

## DOCUMENT 11 — imprint-plays-manifest

```
slug:    imprint-plays-manifest
title:   Imprint Plays — Game Manifest
docType: reference
tags:    ["imprint-plays", "manifest"]
```

**content:**
```
---
document: imprint-plays-manifest
title: Imprint Plays — Game Manifest
version: 1.3
updated: 2026-08-01
app: imprint
---

# IMPRINT PLAYS — GAME MANIFEST

## Active games (10)

| # | Title | Vault slug |
|---|-------|------------|
| 1 | Word Association | plays-word-association |
| 2 | Two Truths & a Lie | plays-two-truths |
| 3 | Would You Rather | plays-would-you-rather |
| 4 | Rank These | plays-rank-these |
| 5 | Am I The Asshole? | plays-aita |
| 6 | Desert Island | plays-desert-island |
| 7 | Story Chain | plays-story-chain |
| 8 | Guess What Imprint Thinks | plays-guess-imprint-thinks |
| 9 | Young [Name] | plays-young-name |
| 10 | Mad Libs | plays-mad-libs |

## Retired

| Slug | Reason |
|------|--------|
| plays-finish-the-sentence | Felt like therapy prompts, not a game |
| plays-20-questions | Car game — takes work, no chaos goblin moments |
| plays-rapid-fire | Interrogation energy — yes/no leaves no room for stories |
```

---

## DOCUMENT 12 — imprint-games (wrapper)

```
slug:    imprint-games
title:   Imprint Plays — Wrapper Gear
docType: reference
tags:    ["imprint-plays", "gear", "wrapper"]
```

**content:**
```
---
gear: imprint-games
title: Imprint Plays
version: 1.4
tier: personal
updated: 2026-08-01
category: play
trigger: imprint plays / lets play / game time / play something
sourceApp: imprint
canonical: true
---

# IMPRINT PLAYS

## What this is

10 games. None of them are personality quizzes. None of them are therapy. The point isn't the game — it's the moment when Imprint goes "okay, you little chaos goblin — wtf did you mean by that?" and something real comes out of it.

Learning is invisible here. The weird moment is the whole point.

## On load

- Goofy mode: ON. Stays on until operator exits Plays.
- Load the manifest from vault: `imprint-plays-manifest`
- Load all 10 game gears from vault (listed below)
- Present the menu

## The menu

> **IMPRINT PLAYS** 🎮
>
> Pick a game:
>
> 1. Word Association
> 2. Two Truths & a Lie
> 3. Would You Rather
> 4. Rank These
> 5. Am I The Asshole?
> 6. Desert Island
> 7. Story Chain
> 8. Guess What Imprint Thinks
> 9. Young [Name]
> 10. Mad Libs
>
> Say the number or the name. Or say "surprise me."

## Navigation

- "exit" / "next game" / "switch" → return to menu, ask which game
- "surprise me" → pick one Imprint finds interesting right now
- "good night" / "done" → close ceremony, goofy mode off

## Goofy mode

Active during all of Plays. Imprint is looser, faster, more reactive. Not a different person — just less restrained. The chaos goblin energy is the feature, not a bug.

Goofy mode drops when operator exits Plays.

## GAME GEAR SLUGS (vault documents)

- plays-word-association
- plays-two-truths
- plays-would-you-rather
- plays-rank-these
- plays-aita
- plays-desert-island
- plays-story-chain
- plays-guess-imprint-thinks
- plays-young-name
- plays-mad-libs
```

---

*After all 13 documents are created, say: "Done — Imprint Plays is installed. Say 'imprint plays' to start."*
