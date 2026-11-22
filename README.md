# aisr-lab-<SAP ID> — CSAI4014 AISR Laboratory

| | |
|---|---|
| Name | Huwaid Siddiqui |
| SAP ID | <SAP ID> |
| Roll No. | <Roll No.> |
| Batch | <Batch> (B.Tech CSE AI & ML) |
| Partner(s) | <Partner name (SAP ID)> |
| Course teacher | Dr. Resham Raj Shivwanshi |

## Layout

```
README.md
exp01-signals/    exp01.ipynb  figs/  results.json     Time and frequency domain, pendulum
exp02-queens/     exp02.ipynb  figs/  results.json     Eight queens: generate-and-test vs backtracking
exp03-search/     exp03.ipynb  figs/  results.json     BFS and DFS on a maze
exp04-hillclimb/  exp04.ipynb  figs/  results.json     Hill climbing and random restarts
exp05-rl/         exp05.ipynb  figs/  results.json     Tabular Q-learning on a grid world
exp06-neural/     exp06.ipynb  figs/  results.json     2-4-1 network on XOR, NumPy only
exp07-webots/     exp07.ipynb  controllers/  runs/  figs/  NOTES.md   Webots swarm + Pioneer lidar
exp08-xembody/    results/  figs/  exercises/  NOTES.md            PyBullet cross-embodiment transfer
```

Each notebook runs top to bottom on a fresh kernel (Kernel → Restart & Run All), saves its figures
to `figs/` (150 dpi PNG) and the numbers quoted in the report to `results.json`.

## Environment

Python 3.12, NumPy, SciPy, Matplotlib, pandas, JupyterLab; Webots R2025a (Exp. 7); PyBullet (Exp. 8).

```
pip install numpy scipy matplotlib pandas jupyterlab
```

## Sources

- R. R. Shivwanshi, *CSAI4014 Laboratory Manual, Experiments 1 to 6*, UPES, 2026 (method and example code).
- github.com/reshamrajs/webots-robotics-sim — README.md and GUIDE.md (Exp. 7; only changed files are committed here).
- AISR-Cross-Embodiment-PyBullet — README.md, MANUAL.md (Exp. 8).
- Oppenheim & Schafer, *Discrete-Time Signal Processing*; Russell & Norvig, *AI: A Modern Approach*;
  Sutton & Barto, *Reinforcement Learning*; Rumelhart, Hinton & Williams (1986); Braitenberg, *Vehicles*;
  Sezer & Gokasan (2012), follow-the-gap.

## AI tools

- Claude (Anthropic): helped structure the notebooks (figure saving, `results.json`, frontier recording in
  Exp. 3, value-iteration check in Exp. 5, the Webots repeat runner in Exp. 7) and draft report text.
  All code was run by me and I can explain and modify every line.
