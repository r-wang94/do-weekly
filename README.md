# Do Weekly — Podcast Production

This directory contains everything needed to produce Do Weekly, a weekly audio programme from Do Health.

## Directory structure

```
podcasts/
├── prompt.md                  # System prompt for script generation
├── timeline.md                # Planned episode themes and theme bank
├── README.md                  # This file
├── episodes/                  # All episodes, one folder each
│   ├── 1_identity/
│   │   ├── concept.md         # Episode brief: theme, pillars, research notes
│   │   ├── script.md          # The written script (~750-850 words)
│   │   └── recording.mp3      # Final recorded audio
│   ├── 2_discomfort/
│   └── ...
└── research/                  # Evolving research bank
    ├── science.md             # Biomarker science, clinical evidence base
    ├── foundations.md         # Distilled, script-ready principles
    ├── voices.md              # Key influences and their core ideas
    ├── quotes.md              # Quotable lines, sticky phrases, listener-ready language
    ├── metaphors.md           # Working metaphors and analogies (used and available)
    └── reading_list.md        # Books, papers, studies to draw from
```

## Episode folder naming

Each episode folder is named `N_theme` where:
- **N** is the episode number (1, 2, 3...)
- **theme** is a single lowercase keyword for the episode (identity, discomfort, tonight...)

Examples: `1_identity`, `2_discomfort`, `6_tonight`

## What goes inside each episode folder

| File | Purpose |
|---|---|
| `concept.md` | Written **before** the script. Captures the theme, which pillar(s) it draws from, key principles, and any episode-specific research, quotes, or references gathered during preparation. |
| `script.md` | The finished script, written using `prompt.md` as the system prompt. |
| `recording.mp3` | The recorded audio of the final script. |

## Two layers of research

### 1. Episode-specific research (`concept.md`)
Each episode's `concept.md` holds research gathered specifically for that script — quotes, references, angles, relevant science. This is the episode brief.

### 2. Evolving research bank (`research/`)
A growing collection of principles, guidance, quotes, books, papers, and references that any episode can draw from. Not tied to a single episode — this bank grows over time.

Additional source material is available outside this directory:
- `/background/` — blogs, books, guides, papers, podcast transcripts
- `/projects/principles/` — full principles documentation

## Workflow

1. Choose a theme from `timeline.md`
2. Create the episode folder (`episodes/N_theme/`)
3. Write `concept.md` — gather episode-specific research, define the angle
4. Generate `script.md` using `prompt.md` as the system prompt, informed by `concept.md` and the research bank
5. Record and save as `recording.mp3`
