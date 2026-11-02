# Module 9: Prompt Engineering and Context Design

Compare prompt instructions and source organization using Phi-4-mini to summarize public-education proposals from four Wake County commissioner candidates. Check whether each claim is relevant and attributed to the correct source.

## Open the lesson

- **[Interactive HTML prompt lab](https://strokeofluck.github.io/Prompt-and-Context-Engineering/)** — build/edit prompts, select candidate sources, inspect source passages, and record answer checks without running a model.
- **[Open the Colab notebook](https://colab.research.google.com/github/Strokeofluck/Prompt-and-Context-Engineering/blob/main/DSA495-M09-Prompt-Context-Engineering.ipynb)** — run actual Phi-4-mini experiments; edit cells directly.
- [Browse the four source TXT files](./knowledgebase/) — versioned candidate materials used by both.

## Contents

| File | Description |
| --- | --- |
| [`DSA495-M09-Prompt-Context-Engineering.ipynb`](./DSA495-M09-Prompt-Context-Engineering.ipynb) | Run Phi-4-mini in Colab and edit the original course exercises. |\n| [`index.html`](./index.html) | Optional interactive browser-based prompt builder and source inspector; no model execution. |\n| [`knowledgebase/`](./knowledgebase/) | Four original candidate TXT source files. |

## What You Will Do

- **Task A:** Use a basic prompt with all four files and check a saved answer against the sources.
- **Task B:** Make persona, instruction, context, format, audience, tone, and data explicit in the prompt.
- **Task C:** Give the model one candidate's file per call and compare attribution and relevance.

Optional activities select relevant excerpts and test the effect of changing one passage-selection decision.

## Before You Begin

Use Google Colab with a **T4 GPU**. The four TXT sources are fetched directly from this repository's `knowledgebase/` folder; **Google Drive is no longer required**.\n\n**Private repository setup:** This repository is currently private. Create a fine-grained GitHub personal access token scoped to this repository with read-only Contents permission, add it to Colab **Secrets** as `GITHUB_TOKEN`, and grant the notebook access to that secret. Never paste a token into the notebook or commit it. If you later make the repository public, the notebook can fetch files without a token.\n\nRun cells in order; complete **Tasks A–C** before optional experiments. Rerun the fetch cell to see new GitHub changes. Set `GITHUB_REF` to a commit SHA instead of `main` to reproduce exactly the same source version.\n\n**GitHub Pages:** The HTML experiment page loads the four source files from `knowledgebase/` and lets you build prompts and inspect evidence interactively; use Colab for real Phi-4-mini inference. Pages must be deployed from `main` at the repository root. The browser page does not need your GitHub token.\n\n**Evidence limitations:** These texts are candidate/campaign self-reports collected October 31, 2026, not independent verification of policy claims.\n