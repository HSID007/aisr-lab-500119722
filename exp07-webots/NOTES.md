# Experiment 7 — notes

Simulator project: `../../webots-robotics-sim` (clone of github.com/reshamrajs/webots-robotics-sim, not re-uploaded here).
Webots R2025a on Windows, Python 3.12.1 virtual environment (`webots-robotics-sim/.venv`).

## Changed files (copied into `controllers/`)

- `tools/run_experiment.py` — Windows fix: the logger output path is written with forward slashes and the
  `re.sub` replacement uses a lambda, otherwise backslashes in the path break the world file. Prints my name and time.
- `analysis/metrics.py`, `controllers/pioneer_lidar_nav/pioneer_lidar_nav.py`,
  `controllers/trajectory_logger/trajectory_logger.py` — print my name and a timestamp with each run.

## Commands

Session runs (13-10-2026, outputs in `runs/session_2026-10-13/`):

```
python tools/run_experiment.py swarm --seconds 120
python tools/run_experiment.py swarm --seconds 120 --set cruise=0.9
python tools/run_experiment.py pioneer --seconds 180
python tools/run_experiment.py pioneer --seconds 180 --set bubble=0.15
```

Repeats and exercises for the report: open `exp07.ipynb` and Restart & Run All. It runs, headless:

- swarm default and cruise=0.9, 3 repeats each (120 s)
- pioneer default, bubble=0.15, k_turn=0.5 (180 s)
- Exercise 1 (GUIDE §10): cruise = 0.2, 0.4, 0.6, 0.8, 1.0, 3 repeats each
- Exercise 4 (GUIDE §10): basicTimeStep = 8, 32, 64 ms, 3 repeats each

CSVs → `runs/`, figures → `figs/`, numbers → `results.json`.
Figure 7.1 is a manual screenshot of `worlds/swarm_arena.wbt` running in the Webots window → `figs/fig7_1_screenshot.png`.
