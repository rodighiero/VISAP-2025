# VISAP 2025 — Lexical Map

A network visualization of the accepted works at [VISAP 2025](https://visap.net/2025/), used in the printed catalog to give an overall view of the submissions presented at the conference.

## How it works

The pipeline extracts noun and proper-noun lemmas from each work abstract using spaCy, builds a TF-IDF matrix across the 26 accepted works, and reduces the resulting high-dimensional space to two dimensions with UMAP (cosine metric). The output is a scatter plot where proximity reflects shared vocabulary and thematic affinity.

## Data

- `data/VISAP.md` — abstracts of the 26 accepted works

## Output

`visap_map.svg` — the final visualization, exported as SVG for print integration.

## Dependencies

```
spacy
scikit-learn
umap-learn
matplotlib
```
