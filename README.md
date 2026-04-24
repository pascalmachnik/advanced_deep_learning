# Advanced Deep Learning in Physics

University coursework repository. Each task produces a Jupyter notebook with code and a short LaTeX report (0.5–1 A4 page).

## Structure

```
advanced_deep_learning/
├── tasks/
│   ├── task_template/   ← copy this to start a new task
│   └── task_01/         ← completed tasks
└── latex_config/        ← shared LaTeX setup
```

## Starting a New Task

```bash
cp -r tasks/task_template tasks/task_XX
```

Then add code to `notebook.ipynb` and write a short report into `report.tex`.

## Build Report

Run from inside a task directory:

```bash
make all      # compile report.tex → build/report.pdf
make preview  # live-recompile on save
make clean    # remove build/
```
