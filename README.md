# Geography + AI: Teaching Notebooks

![overview](assets/overview.png)

A growing, open collection of reproducible Jupyter notebooks for **bringing AI and computational methods into geography teaching**. Each notebook is a self-contained teaching module: it pairs a clear narrative with runnable code, so that students — and other instructors — can learn by executing every cell.

Maintained by **Jun-Yi Lee (李俊逸)**, a hydrologist and geographer. The collection is updated over time as new datasets, methods, and classroom-tested patterns are added.

## Why this repository exists

Geography students increasingly need to read data, write a little code, and use AI tools critically. These notebooks are designed around three principles:

1. **Runnable anywhere** — every notebook uses only standard scientific Python (NumPy, SciPy, scikit-learn, Matplotlib) and synthetic or openly described data. No licensed software, no API keys.
2. **Narrative first** — the markdown cells explain *why*, not just *how*, so a notebook can be read like a short chapter.
3. **AI as a thinking tool, not an oracle** — where AI is used, students are asked to evaluate and critique its output, never to accept it blindly.

## Notebooks

| # | Notebook | Topic |
|---|---|---|
| 1 | `notebooks/01_rainfall_pattern_ml.ipynb` | Classifying storm rainfall patterns with machine learning |
| 2 | `notebooks/02_watershed_gis_python.ipynb` | Watershed analysis from a DEM with pure Python |
| 3 | `notebooks/03_ai_in_geography_teaching.ipynb` | Generative AI as a geography-teaching companion |

Each notebook works on its own; there is no required order.

## Running the notebooks

```bash
git clone https://github.com/junyilee7/geography-ai-teaching.git
cd geography-ai-teaching
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter lab
```

GitHub also renders `.ipynb` files in the browser, so the notebooks can be read without running anything.

## Topics covered

- Unsupervised learning (PCA, k-means) on spatial fields
- Digital elevation model analysis: flow direction, flow accumulation, stream networks, hypsometry, wetness index
- Practical patterns for using large language models and vision models in the classroom
- Critical evaluation of AI output as a learning objective

## Roadmap

This repository is a living resource. Planned additions include notebooks on remote-sensing image classification, time-series forecasting for hydrology, and open-data workflows. Suggestions are welcome via Issues.

## Citation

> Lee, J.-Y. (2026). *Geography + AI: Teaching Notebooks*. GitHub. https://github.com/junyilee7/geography-ai-teaching

## License

Released under the [MIT License](LICENSE). The educational narratives in the markdown cells may be reused in teaching with attribution.
