# AI Survey Workflows with EDSL — Week 5 Workshop

Materials for hands-on lab on building AI-powered survey experiments using the [Expected Parrot Domain-Specific Language (EDSL)](https://github.com/expectedparrot/edsl) framework.

---

## Files

| File | Purpose |
|------|---------|
| `edsl_workshop.ipynb` | **Main notebook** — step-by-step coding tutorial for students |
| `edsl_workshop_slides.pptx` | **Lecture slides** |

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

## Workshop Agenda 

| Activity |
|---------|
| Setup & imports |
| Core concepts walkthrough (slides) |
| Live demo — full pipeline in the notebook |
| Hands-on exercises (pairs) |
| Wrap-up & Q&A |

---

## Individual Assignment: The Replication Game - OPTIONAL

Each student will replicate a published survey finding from a major social science data source (GSS, Pew, ANES, etc.) by:

1. Identifying a published survey question with a demographic breakdown
2. Building EDSL agents that match the human sample's demographics
3. Running the survey and comparing AI vs. human response distributions
4. Submitting a written report with figures and interpretation

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
