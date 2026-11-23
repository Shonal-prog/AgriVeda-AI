# AgriVeda — AI-Driven Agricultural & Mandi Simulation

AgriVeda is a Python-based agricultural simulation project exploring farm-level decision-making, resource management, and mandi market dynamics. The project was developed as part of **Smart India Hackathon 2025 (Round 2)**.

## Project highlights

- Custom agricultural simulation environments built with Python, NumPy, and Gymnasium.
- A PPO (Proximal Policy Optimization) training experiment using Stable-Baselines3 in the initial single-agent farm environment.
- A multi-agent simulation representing competing farmer agents and shared market conditions.
- A rolling-window mandi price forecasting component using historical simulated prices and NumPy-based trend fitting.
- Gradio interface components for interacting with the simulation.
- Jupyter Notebook-based experimentation and implementation.

> **Scope note:** PPO training is present in the initial single-agent environment. The notebook also contains later multi-agent simulation code; this repository does not claim that PPO trains the later multi-agent environment.

## Technology stack

- Python
- NumPy
- Gymnasium
- Stable-Baselines3
- Gradio
- Matplotlib
- Pandas
- Jupyter Notebook
- LangChain Google GenAI integration (optional; requires a user-provided API key)

## Repository contents

- `AgriVeda_Simulation.ipynb` — cleaned notebook with saved outputs removed and hardcoded credentials scrubbed.
- `requirements.txt` — Python dependencies used by the notebook.
- `.gitignore` — excludes local environments, notebook checkpoints, and secret files.

## Run locally

1. Clone this repository:

   ```bash
   git clone https://github.com/Shonal-prog/AgriVeda-AI.git
   cd AgriVeda-AI
   ```

2. Create and activate a virtual environment:

   ```bash
   python -m venv .venv
   ```

   Windows PowerShell:

   ```powershell
   .venv\Scripts\Activate.ps1
   ```

   macOS/Linux:

   ```bash
   source .venv/bin/activate
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Start Jupyter:

   ```bash
   jupyter notebook
   ```

5. Open `AgriVeda_Simulation.ipynb` and run the cells in order.

## Optional Gemini integration

Some notebook cells contain an optional Google Gemini / LangChain integration. To use it, create your own API key in Google AI Studio and set it as an environment variable. Never commit API keys to GitHub.

Windows PowerShell:

```powershell
$env:GOOGLE_API_KEY="your-key-here"
```

macOS/Linux:

```bash
export GOOGLE_API_KEY="your-key-here"
```

If you do not configure a key, skip the optional LLM-dependent cells.

## Notes

- This is an experimental simulation, not a production agricultural advisory or financial forecasting system.
- Market prices and environmental conditions are simulated; forecasts should not be interpreted as real mandi price predictions.
- Results depend on simulation assumptions, random initialization, and the selected parameters.

## Author

**Shonal Dhauni**  
GitHub: [@Shonal-prog](https://github.com/Shonal-prog)
