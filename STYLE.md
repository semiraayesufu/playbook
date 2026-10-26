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
| `claim` | Bold takeaway | **The point of the tool as a statement, under 12 words.** Not a label. ("Most strengths can be copied by next year.") |
| `why` | Paragraph under the claim | Why the tool matters and what goes wrong without it. Three to five sentences |
| `ask` | Questions to ask | 3 short questions a reader asks before starting. Don't repeat the steps word for word |
| `steps` | Steps | Numbered actions, each starting with a verb. Sub-lists for options or criteria |
| `example` | In practice | One running example per playbook, carried through every tool, with real numbers |
| `outcome` | By the end | What the reader walks away with. Finishes the sentence "By the end you'll have…" or "…know…", written as a noun phrase |
| `watch` | Watch out | The most common way the tool is misused, in one or two sentences |
| `skip` | Skip it when | When not to use the tool, and which tool to use instead if there is one |

`claim`, `ask`, `outcome` and `skip` are optional for backward compatibility, but every
rewritten tool should have all four.

## Borrowed from the PAIR Guidebook

- **Headings that state the point.** The `claim` is a takeaway, not a topic.
- **Guiding questions** before the method, so readers frame the problem first.
- **A named outcome**, so every tool has a finish line.
- **Named dimensions.** Break a judgement into labelled factors with one sentence each.
- **Balance.** Say when a tool fits and when another one fits better.

## Not borrowed

- Hedging ("it's important to", "consider"), repeated sentences and abstract nouns
  ("socio-technical drivers", "inflection points").

## Before you edit

- Run `git pull` first. Edits made on an old copy of `index.html` have undone newer work
  several times.
- Keep these unless asked: 3-column homepage cards (`.home .in`, `.feed`), playbook search
  (`data-pb`), and the About quote "A moving woman will surely meet her luck."
