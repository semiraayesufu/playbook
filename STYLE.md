# The MBA Playbook style guide

How every tool, playbook intro and glossary entry is written. Benchmarks: the
[People + AI Guidebook](https://pair.withgoogle.com/guidebook/) for structure, and this
playbook's own running examples for voice.

## Voice

- Write for a busy MBA student or manager who wants to use the tool today.
- Plain words over jargon. If a term is needed, define it in the same sentence.
- Direct verbs. Write "Rate each force", not "It's important to consider rating each force".
- Confident, not hedged. Cut "it's important to", "consider", "may want to", "in order to".
- One idea per sentence. Mix short and medium sentences. Split anything over about 30 words.
- Say each thing once. If two sentences make the same point, keep the sharper one.

## Mechanics

- UK spelling: organise, organisation, labour, licence (noun), programme.
- No colons inside prose sentences. Colons are fine after a bold label in a list
  (`**Rare:** do few competitors have it?`) and to introduce a list.
- No middots (·). Use commas.
- Never "something". Name the thing.
- Numbers as figures (3 tools, 40%, $30 a month). Write arithmetic with signs (`$2m − $1.5m = $0.5m`).
- Bold (`**…**`) only for terms the reader must remember, a few per tool at most.
- No AI tells: no "delve", "leverage", "robust", "seamless", "crucial", "in today's world",
  "not just X but Y", rhetorical questions as openers, or lists of three adjectives.

## Anatomy of a tool

Each tool object in `index.html` has these fields, rendered in this order.

| Field | Shows as | Rule |
|---|---|---|
| `name` | Title | The framework's common name |
| `what` | Line under the title | One sentence, under 12 words, starts with a verb ("Tests whether…") |
| `def` | What it is | Two or three sentences. What it is and where the name comes from |
| `why` | Second paragraph of What it is | Why the tool matters and what goes wrong without it. Three to five sentences |
| `steps` | Steps | Numbered actions, each starting with a verb. Sub-lists for options or criteria |
| `example` | In practice | One running example per playbook, carried through every tool, with real numbers |
| `watch` | Watch out | The most common way the tool is misused, in one or two sentences |

Don't add takeaway, questions-to-ask, "By the end" or "Skip it when" sections. They were
tried on Strategy and dropped.

## Borrowed from the PAIR Guidebook

- **Lead with the point.** Open the `why` paragraph with its takeaway, not with background.
- **Named dimensions.** Break a judgement into labelled factors with one sentence each.
- **Balance.** Say when a tool fits and when another one fits better, inside the existing fields.

## Not borrowed

- Hedging ("it's important to", "consider"), repeated sentences and abstract nouns
  ("socio-technical drivers", "inflection points").

## Before you edit

- Run `git pull` first. Edits made on an old copy of `index.html` have undone newer work
  several times.
- Keep these unless asked: 3-column homepage cards (`.home .in`, `.feed`), playbook search
  (`data-pb`), and the About quote "A moving woman will surely meet her luck."
- A local Git check (`.git/hooks/pre-commit`, on Semira's Mac) refuses any commit of
  `index.html` that is missing one of these. If it stops you, pull and reapply your edits.
