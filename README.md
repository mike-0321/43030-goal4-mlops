# Goal 4: Basic MLOps

A local digits classifier for training, experiment tracking, API prediction and model recovery.

Use Python 3.12 and Git. From a fresh clone's root:

```sh
python3.12 -m venv .venv
.venv/bin/python -m pip install -r requirements.lock
.venv/bin/python -m learning_service.train
.venv/bin/python -m pytest -v
.venv/bin/python -m learning_service.recovery
.venv/bin/python -m learning_service.observations
```

Optional interactive API after training:

```sh
.venv/bin/python serve_demo.py
```

On Windows, replace `.venv/bin/python` with `.venv\Scripts\python.exe`.

Data: UCI Optical Recognition of Handwritten Digits, [DOI: 10.24432/C50P49](https://doi.org/10.24432/C50P49).

This public-digits exercise runs locally; its results do not establish clinical performance.
