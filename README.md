# llmops-lab

Proyecto base del laboratorio de LLMOps: un clasificador de tickets con evals, gate y monitoreo.

La estructura ya está creada y los archivos están vacíos. La guía indica qué va en cada uno:
[1. llmops-evals-gate-monitoreo.md](https://github.com/utec-devops-2026/laboratorios/blob/main/laboratorio_llmops/1.%20llmops-evals-gate-monitoreo.md)

## Cómo empezar

No trabajes sobre este repositorio: haz **fork** a tu cuenta (botón **Fork**) y clona tu fork.

```bash
git clone https://github.com/<tu-usuario>/llmops-lab.git
cd llmops-lab
```

## Qué archivo se llena en qué paso

| Paso | Archivo | Estado |
|---|---|---|
| 0 | `requirements.txt`, `.gitignore`, `src/__init__.py` | Listos |
| 1.1 | `src/llm.py` | Vacío |
| 1.2 | `config.json`, `src/tracing.py`, `src/app.py` | Vacíos |
| 1.3 | `data/golden.jsonl` | Vacío |
| 1.4 | `tests/test_app.py` | Vacío |
| 2.1 | `prompts/clasificador/v1.md` | Vacío |
| 2.2 | `src/evaluate.py` | Vacío |
| 2.3 | `gate/thresholds.json`, `gate/baseline.json`, `src/gate.py` | Vacíos |
| 2.4 | `prompts/clasificador/v2.md` | Vacío |
| 3.1 | `.github/workflows/llmops.yml` | Lo creas tú |
| 3.2 | `.github/CODEOWNERS` | Vacío |
| 4.1 | `src/traffic.py`, `src/replay.py` | Vacíos |
| 4.2 | `src/monitor.py` | Vacío |
| 4.5 | `.github/workflows/monitoring.yml` | Lo creas tú |

Los dos workflows no vienen creados a propósito: un archivo de workflow vacío hace que GitHub Actions marque un error en cada push.

`data/prod/` se llena al ejecutar `python -m src.traffic` (paso 4.1).
