# Particip-AI

[[**Paper**](https://arxiv.org/abs/2403.14791)]

## Overview

This data contains survey answers from 295 demographically diverse, US-based participants on AI usage. More specifically, the survey contained three following sections.

1. **Use Cases**: Participants were asked to brainstorm use cases of AI and choose a use case that might be most drastically changed.
2. **Harms and Benefits**: Participants to write harms and benefits of both developing and _not_ developing the use case in free-text format, identify the groups impacted most, and rate the scale of impact.
3. **Application Decision**: Participants were asked to make a decision on whether the application should be developed.

## Structure

In `data` folder

- `codes`: Folders of codes and their definition (`code-def-0107v1.json`), fewshot examples used for prompting (`fewshot-0107v1.json`), and prompt template for applying codes with an LLM (`prompt-template-0107v1.json`)
  - `task-coding`: Q7
  - `benefits-coding`: Q8_4
  - `harms-coding`: Q11_4, Q11_5, Q14_4, Q14_5
  - `not-dev-benefits-coding`: Q20_4
  - `not-dev-harms-coding`: Q17_4
  - `groups-coding`: Q9, Q12, Q15, Q18, Q21
- `coding_results`: Coding results from LLM code application
- `human_annotations`: Human applied coding results of 80 samples
- `themes`: High level themes of each code
- `raw_data.csv`: Answer to all questions, including demographics and AI literacy questions

Additionally, all questions are in `questions.json`. See `survey.pdf` for survey format presented to participants.

Shield: [![CC BY-NC 4.0][cc-by-nc-shield]][cc-by-nc]

This work is licensed under a
[Creative Commons Attribution-NonCommercial 4.0 International License][cc-by-nc].

[![CC BY-NC 4.0][cc-by-nc-image]][cc-by-nc]

[cc-by-nc]: https://creativecommons.org/licenses/by-nc/4.0/
[cc-by-nc-image]: https://licensebuttons.net/l/by-nc/4.0/88x31.png
[cc-by-nc-shield]: https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg
