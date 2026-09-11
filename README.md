# IntroInfo_2026_02_Ucaldas

Curso de Introducción a la Informática (40G8F) en la Universidad de Caldas 2026-2, renovado con una herramienta de IA por sesión.

📖 Libro publicado: https://bioaiteamlearning.github.io/IntroInfo_2026_02_Ucaldas/

El libro se construye y publica automáticamente con GitHub Actions en cada push a `main` (ver `.github/workflows/deploy.yml`).

## Construir el libro

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
jupyter-book build .
```

## Publicar manualmente (si hiciera falta)

```bash
ghp-import -n -p -f _build/html
```
