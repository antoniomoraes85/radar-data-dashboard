# Radar Data — Traffic Accident EDA Prototype

**Python · Pandas · Matplotlib · Seaborn · Jupyter**

A small exploratory notebook for grouping and visualizing traffic-accident records by **Brazilian state (UF)**, **hour of day**, and **vehicle type**.

This repository is an **early data-analysis prototype**, not a deployed interactive dashboard or a completed study of official PRF datasets.

## Implemented

The notebook [`radar_analysis.ipynb`](radar_analysis.ipynb) currently:

- Reads a semicolon-delimited CSV using Latin-1 encoding.
- Displays descriptive information about the data.
- Plots accident counts by `uf`, `horario`, and `veiculo`.
- Prints total records and the three most frequent state labels.

## Dataset and reproducibility

The notebook expects a CSV at **`../data/acidentes_exemplo.csv`** relative to its execution directory, containing at least the columns:

| uf | horario | veiculo |
| --- | --- | --- |
| RS | 8 | Automóvel |
| SC | 14 | Motocicleta |

The two rows above are **illustrative examples, not observed accidents**. The input CSV is **not included** in this GitHub repository. The executed notebook contains output from a small example dataset; it is **not** evidence of a national accident survey.

To run this notebook, supply your own authorized dataset with those fields, adapt the path as necessary, install `pandas`, `matplotlib`, `seaborn`, and `jupyter`, and execute the cells.

## Planned improvements

1. Include a clearly labeled synthetic example CSV and make file paths relative to the repository.
2. Add an import/validation pipeline for documented public datasets, including source, period, and schema.
3. Add reproducible tests for data cleaning and aggregation.
4. Implement interactive filtering and maps only after the dataset pipeline is validated.
5. Publish reproducible figures, limitations and a concise results report.

## Author

José Antônio Coutinho de Moraes Filho · [GitHub](https://github.com/antoniomoraes85) · [LinkedIn](https://www.linkedin.com/in/joseantoniomoraes/)
