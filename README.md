# Clustering countries by development indicators

> Course assignment from 2023, kept as it was written. The notes under "Reading the result" were added in November 2026.

Groups 167 countries into three development levels from nine socio-economic and health
indicators, with K-means, Ward hierarchical clustering and PCA.

## Method

1. Clip outliers to 1.5 IQR and standardise the nine indicators.
2. K-means with k = 3 and Ward agglomerative clustering with 3 clusters.
3. Name the clusters by looking at their members.
4. Reduce the four social and the five economic indicators to one PCA score each, to plot countries
   on two axes.

## Result

| Group | K-means | Hierarchical |
|---|---|---|
| Developed | 41 | 71 |
| Developing | 79 | 61 |
| Underdeveloped | 47 | 35 |

## Reading the result

- The two methods agree on the poorest group and disagree on where "developing" ends: 41 or 71
  developed countries. The groups are a rough ordering, not a classification.
- k = 3 was given by the brief. The notebook does not test whether the data supports three groups.

## Files

| File | Content |
|---|---|
| `Country_Clustering.ipynb` | Analysis |
| `Country_Clustering.html` | Rendered copy |
| `Country-data .csv` | The dataset |
| `About.txt` | Original brief and column descriptions |
