# ML Gym

Hands-on, generic AI/ML practice repo organized by tiers.
Each project lives in `/projects` and produces a small, finished artifact.

## Structure
- `projects/` — mini-projects by tier
- `src/ml_gym/` — reusable utilities (metrics, viz, IO, pipelines)
- `docs/` — progress tracker + notes
- `data/` — datasets (raw data is gitignored)

## Getting Started
```bash
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
python -m ipykernel install --user --name ml-gym
jupyter lab
