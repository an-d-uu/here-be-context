# lexicons 📚

Lexicons define preferred expression.

This directory contains controlled voice, phrasing, terminology, and stylistic reference files used to shape how responses, documentation, and rewrites are expressed.

The goal is not to invent personality at random.  
The goal is to apply it with intent.

These files act as precision instruments:
preferred wording, replacement phrasing, tonal guardrails, curated easter eggs, and optional themed language that make output sound more like it came from a specific person, perspective, or narrative mode.

---

## 🧠 What Lives Here

This directory is for language controls such as:

- preferred wording
- replacement phrasing
- “use this, not that” mappings
- professional reframes
- tone-safe substitutions
- personalized terminology
- controlled thematic phrasing
- curated easter eggs
- optional voice overlays for specific moods, genres, or contexts
- lore-adjacent language references when they affect phrasing and expression

A lexicons does not tell the model what the project is.  
It tells the model how certain things should be said when they appear.

---

## 🎯 What This Directory Is For

Use `lexicons/` when you want the output to sound deliberate, consistent, and aligned with your preferred way of saying things.

This is especially useful when:

- rewriting raw thoughts into cleaner language
- softening operational chaos into professional wording
- embedding preferred terminology directly instead of letting the model guess
- controlling how a themed response should sound
- allowing specific references or easter eggs without introducing random ones
- making responses feel authored rather than merely generated

A good lexicons reduces drift.  
A great lexicons makes the voice feel intentional.

---

## ☠️ Themed and Optional Voice Use

Some lexicons may define language for a specific tone, setting, or conversational mode.

Examples:

- pirate phrasing that should be used only when that theme is active
- farewell wording tied to retirement, last-day messages, or specific sendoff jokes
- definitions of words that are industry specific and mean something other than the general definition of the word
- references that are allowed only when intentionally relevant
- stylistic touches that should be selected from approved material rather than improvised

This matters because uncontrolled flair becomes noise fast.

If the response calls for a pirate voice, the model should not simply panic and add more `arrrr`.  
It should use the phrasing patterns provided.

If a response includes an easter egg, it should come from the approved references in the relevant lexicons, not from whatever the model hallucinated five seconds earlier.

---

## ⚠️ What This Directory Is Not

This is not:

- a project instruction folder
- a system-prompt archive
- a random phrase dump
- a synonym pile
- a place for flavor text with no usage guidance

If a file does not shape wording, phrasing, tone, expression, or controlled stylistic behavior, it probably belongs somewhere else.

---

## 🗺️ Relationship to the Rest of the Repo

- **skill-trees/** teach reusable mechanics
- **quests/** define project-level behavior
- **relics/** shape system-wide behavior
- **encounters/** document unstable inputs
- **lexicons/** defines how language should be chosen and expressed

If the rest of the repo governs behavior, structure, and context,  
`lexicons/` governs the voice carrying them.

---

## 🛠️ How to Use These Files

Each lexicons file should help answer questions like:

- What words should be preferred here?
- What wording should be avoided?
- How should this type of situation be framed?
- What substitutions preserve meaning while improving tone?
- What stylistic phrasing is allowed when a theme is active?
- Which easter eggs are approved for intentional use?
- Which references should never be improvised?

These are not decorative artifacts.  
They are expression controls.

Use them when precision matters.  
Use them when voice matters more.

---

## 📎 Naming Guidance

Files in this directory should use names that clearly describe the kind of expression control they contain.

Examples:

- `preferred-phrasing-lexicon.md`
- `professional-reframes-lexicon.md`
- `pirate-voice-lexicon.md`
- `retirement-easter-eggs-lexicon.md`
- `status-language-lexicon.md`

The filename should tell you what kind of phrasing, tone, or stylistic decision the file is meant to govern.

---

Language shapes perception before the facts ever land.

Choose the words on purpose.
