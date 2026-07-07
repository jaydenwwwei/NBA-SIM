# NBA SIM

An NBA-themed Streamlit app with two modes:

- Team Simulator: projects a score, winner, MVP, player box scores, and themed stat charts.
- Find My NBA Match: compares your per-game profile with NBA player seasons using a random-forest model.

## Run locally

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
streamlit run streamlit_app.py
```

On macOS or Linux, activate the environment with `source .venv/bin/activate`.

## Deploy on Streamlit Community Cloud

Choose this repository, the `main` branch, and `streamlit_app.py` as the app entry point. No secrets are required.

The player-matching model is trained and cached automatically on first use. Team simulations retrieve current NBA data through `nba_api`.
