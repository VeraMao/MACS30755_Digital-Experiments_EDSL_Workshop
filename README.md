# AI Survey Workflows with EDSL — Week 5 Workshop

Materials for hands-on lab on building AI-powered survey experiments using the [Expected Parrot Domain-Specific Language (EDSL)](https://github.com/expectedparrot/edsl) framework.

---

## Files

| File | Purpose |
|------|---------|
| `edsl_workshop.ipynb` | **Main notebook** — step-by-step coding tutorial for students |
| `edsl_workshop_slides.pptx` | **Lecture slides** — 13-slide deck for the 80-min session |
| `edsl_instructor_guide.docx` | **Teaching guide** — timing, demo script, rubric, common pitfalls |

---

## What Students Will Learn

By the end of the session, students can:

- Install and configure EDSL with LLM API keys
- Create survey questions (MultipleChoice, YesNo, LinearScale, FreeText, CheckBox)
- Build AI agent personas with demographic traits (party, age, education, region…)
- Specify and compare language models (GPT-4o, Claude, Gemini)
- Run multi-agent surveys with the `.by()` pipeline and extract results
- Produce AI vs. human comparison visualizations for the replication game assignment

---

## Setup (Students)

**1. Install EDSL**
```bash
pip install edsl
```
Requires Python 3.9–3.12.

**2. Set an API key** (at least one provider required)
```bash
export OPENAI_API_KEY="sk-..."          # OpenAI / GPT
export ANTHROPIC_API_KEY="sk-ant-..."   # Anthropic / Claude
export GOOGLE_API_KEY="AIza..."         # Google / Gemini
```

**3. Open the notebook**
```bash
jupyter lab edsl_workshop.ipynb
```
Or upload to [Google Colab](https://colab.research.google.com/) and run `!pip install edsl` in the first cell.

---

## Workshop Agenda (80 min)

| Time | Activity |
|------|---------|
| 0:00 – 0:10 | Setup & imports |
| 0:10 – 0:25 | Core concepts walkthrough (slides) |
| 0:25 – 0:45 | Live demo — full pipeline in the notebook |
| 0:45 – 1:10 | Hands-on exercises (pairs) |
| 1:10 – 1:20 | Replication game assignment preview |
| 1:20 – 1:30 | Wrap-up & Q&A |

---

## Individual Assignment: The Replication Game - OPTIONAL

Each student will replicate a published survey finding from a major social science data source (GSS, Pew, ANES, etc.) by:

1. Identifying a published survey question with a demographic breakdown
2. Building EDSL agents that match the human sample's demographics
3. Running the survey and comparing AI vs. human response distributions
4. Submitting a written report with figures and interpretation

Full rubric and guidance are in `edsl_instructor_guide.docx` and in **Section 8** of the notebook.

---

## Recommended Data Sources

- **GSS Data Explorer** — [gssdataexplorer.norc.org](https://gssdataexplorer.norc.org/)
- **Pew Research Datasets** — [pewresearch.org/datasets](https://www.pewresearch.org/datasets/)
- **ANES** — [electionstudies.org](https://electionstudies.org/data-center/)
- **IPUMS** — [ipums.org](https://www.ipums.org/)

---

## Key References

- Argyle et al. (2023). "Out of One, Many: Using Language Models to Simulate Human Samples." *Political Analysis.*
- Santurkar et al. (2023). "Whose Opinions Do Language Models Reflect?" *ICML.*
- Bisbee et al. (2023). "Synthetic Replacements for Human Survey Data? The Perils of Large Language Models." *Political Analysis.*
- Smith et al. (2023). *General Social Surveys, 1972–2022.* NORC at the University of Chicago.

---

## EDSL Resources

- Docs: [docs.expectedparrot.com](https://docs.expectedparrot.com/)
- GitHub: [github.com/expectedparrot/edsl](https://github.com/expectedparrot/edsl)
