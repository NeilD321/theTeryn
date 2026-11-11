# Architecture

Status: **PROPOSAL. Nothing in this file is approved.** Approved items move to `DECISIONS.md`.

---

## 1. Hierarchy

Proposed:

```text
The Teryn
└── Parts (5–7 broad groupings)               ← proposed addition
    └── Books (each independently readable)
        └── Chapters (titled, numbered)
            └── Verses (numbered)
```

Why add **Parts**:

- With 20 or more books, readers need orientation.
- The Bible has its two Testaments; the Tanakh has its three sections.
- Parts give the whole an arc, so it is a journey and not a list.

Parts are for navigation only. They never appear in references.

Inside chapters, **section headings** are allowed for readability. As in modern Bibles, they are not part of the referenced text.

## 2. Overall arc

Three organising principles were considered:

| Option | Shape | Strength | Weakness |
|---|---|---|---|
| A. Thematic | Subject groupings in any order | Flexible | No narrative pull; feels like an encyclopaedia |
| B. Cosmic arc | Universe → life → us → society → future | Honest counterpart to Genesis → Revelation; a real story with a real beginning and an open ending | Personal subjects sit in the middle |
| C. A life's arc | Birth → childhood → love → work → age → death | Intimate, universal | Hard to fit science, society and the future |

**Recommendation: B, with C nested inside it.** The whole collection follows cosmic time, from the beginning of the universe to the open future. The "Being Human" part follows a single life from birth to death.

Proposed parts (working names):

1. **Origins**: what there is, and how it came to be.
2. **Knowing**: how we found out, how we think, how we get it wrong. Placed second because it answers "how do you know?", the question Part 1 provokes.
3. **Being Human**: the arc of a single life.
4. **Living Well**: how to treat ourselves and each other.
5. **Together**: communities, civilisation, power, history.
6. **Voices**: individual contributors, letters and testimony.
7. **Tomorrow**: what we owe the future, and what it might hold. It closes the arc that Origins opened.

There is also a short, welcoming **opening** before Part 1, built around the founding line (see `VISION.md`).

## 3. Book naming

Options:

- **Subject-named** ("The Book of Mortality"). Timeless, neutral, easy to cite. Can feel abstract.
- **Person-named** ("The Book of Ricky"). Personality and marketability. But it ties the work to living reputations, dates quickly, needs permission, and reads oddly in references ("Ricky 4:3").
- **Mixed**.

**Recommendation: subject names for every book, with attribution where a book has an author.**

- *The Book of Laughter*, written by [contributor].
- Contributor pieces live mainly in Part 6 (**Voices**), modelled on the epistles: *A Letter on Doubt*, from [contributor].
- Person-named books are reserved, if used at all, for **historical figures whose actual words** form the book.

See `CONTRIBUTOR_CONCEPTS.md` for the full reasoning.

Naming rules (proposed):

- Every book has a **one-word short name**, unique and not a prefix of another (*Laughter*, *Kin*, *Doubt*).
- Every book has a 3–4 letter abbreviation (*Lau*, *Kin*, *Dbt*).
- Avoid "The Book of Life": it is too broad, and close to the project's own tagline.

## 4. Verses

### Principle: write the text first, then lay the grid

The Bible's numbering was imposed centuries after writing. Ours is applied by the editor after a passage is drafted, but deliberately, using rules.

**Verse rules (proposed):**

1. A verse is **one complete thought**, usually one sentence, occasionally two short ones.
2. **Never break mid-sentence.**
3. Target length: **10–40 words**. Hard cap about 60 words; split longer sentences at the writing stage, not the numbering stage.
4. Chapters aim for **10–60 verses**, readable in one sitting. The Bible averages about 26.
5. Verse numbering must not change the writing. If a passage only "works" because each sentence has been forced into a quotable aphorism, rewrite it as prose.

> **Founder's direction (28 Oct 2026):** no long paragraphs anywhere. All writing is short, meaningful verses, each on its own line, and chapters must still read straight through. The "Prose" layout mode below is therefore dropped, and rule 3's word limits should come down. The other modes remain possibilities.

### Layout modes

Each book declares one or more layout modes:

| Mode | Use | Presentation |
|---|---|---|
| **Saying** | Aphoristic, wisdom books | Each verse its own line |
| **Prose** | Narrative, science, argument | Normal paragraphs with small superscript verse numbers inline |
| **Poem** | Poetry, lament | Lines and stanzas; verse = sentence or stanza, set per book |
| **Dialogue** | Debates, Q&A, dilemmas | Each speaker's turn is a verse |
| **List** | Practical guidance, catalogues | Numbered items = verses |

The prose mode is what keeps scientific and narrative books readable. A reader sees paragraphs; a citer sees numbers.

### Avoiding the scripture voice

The Bible's English cadence leaks in easily: verses beginning "And…", "Nor…", "For…"; inversions; solemnity. Grayling's *The Good Book* shows how strong the pull is (see `RESEARCH/prior-art.md`). House rule (proposed): **no verse may begin with a conjunction purely for rhythm**, and drafts are read aloud as ordinary prose to check they sound like a person, not a pulpit.

### Verses as a fact-checking unit

For factual books, each verse can carry source notes keyed to its reference. This gives The Teryn something a conventional book lacks: **every factual claim is individually addressable, sourced and correctable.**

## 5. Referencing

| Form | Example | Use |
|---|---|---|
| Short (standard) | **Humanity 4:3** | Everyday citation |
| Full | **Teryn, Humanity 4:3** | First mention, outside contexts |
| Edition-specific | **Humanity 4:3 (T1)** or **(2027 ed.)** | When exact wording matters |
| Range | **Humanity 4:3–7**, **Humanity 4:3–5:2** | |
| Machine ID | `HUM.4.3` | Digital editions, links, databases |

Rejected: **Teryn 5:4:3** (book numbers). Numbers are unmemorable, and book order may change as books are added, which would break every citation. Books are always cited by name.

## 6. Living collection: stability rules

The tension: The Teryn should evolve as knowledge changes, but references must never break.

**Proposed guarantees:**

1. **Editions** are numbered and dated (First Edition, 2027; Second Edition…). Every published edition is archived permanently.
2. **Book identifiers are permanent** and never reused, even if a book is withdrawn.
3. **Chapter and verse numbers are never reassigned.** New chapters are appended at the end of a book. New verses are appended at the end of a chapter, or the chapter is replaced.
4. **Withdrawn verses keep their number** and are marked *"[Withdrawn in Edition 3 — see notes]"*. Modern Bibles do the same with omitted verses such as Acts 8:37.
5. **Wording may be revised** between editions; the reference stays and the change is logged.
6. **Two kinds of change:**
   - *Corrections*: factual errors, fixed promptly and logged in published errata.
   - *Revisions*: substantive changes, made only in new editions, through the editorial process.
7. **Major rewrites** become a new chapter; the old one is retired, not overwritten.
8. **Candidate books** can be published openly outside the core collection before admission (our equivalent of the apocrypha, without the stigma).
9. Every passage has a **public revision history**. This repository, kept under version control, is the natural foundation for that.

## 7. Apparatus (eventual)

- Opening: how to read The Teryn
- Contents, and a contents by Part
- Source notes keyed to verses
- Cross-references
- Concordance or index
- Revision history and errata
- Reading plans (a passage a day, a book a month)

Physical design (typography, page layout, editions) is deferred until content exists, but layout modes (section 4) should be fixed early because they affect writing.

## 8. Recommended starting architecture (summary)

- **Shape:** opening + 7 Parts, following cosmic time, with a life's arc in the middle.
- **Books:** subject-named, one-word short names. Contributors are credited, not titled.
- **First Edition target:** about **12–16 books**, deliberately varied in voice. Not all 40 or so brainstormed ideas.
- **Verses:** sentence-level units, five layout modes, a prose-first writing process.
- **References:** `Book C:V`, with an optional edition tag. Machine IDs for digital use.
- **Change:** editions, permanent numbering, withdrawn verses kept, public history.

## 9. Decisions needed before writing begins

See `DECISIONS.md`, "Open decisions".
