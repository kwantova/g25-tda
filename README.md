# g25-tda

# Topological Data Analysis of human genetic diversity

Mapper graph based on Eurogenes Global 25 (G25) coordinates.  
The dataset contains **10,927** individual samples, **1,003** named populations, **25** dimensions

📒 See the interactive version here:\
https://kwantova.github.io/g25-tda/
---

## Interactive visualization

### Graph navigation
- **Mouse wheel** — zoom in / zoom out
- **Drag** — pan across the canvas
- **Double-click on empty space** — reset zoom and return to the default view
- **Double-click on legend** — isolate one region, hiding all others

### Working with nodes
- **Hover over a node** — tooltip with the region name and the full list of populations within that topological cluster
- **Click on a node** — pin the tooltip so you can scroll through the population list
- **Escape** — close the pinned tooltip
- **Scroll inside the tooltip** — the population list is scrollable when there are more than 12 entries

### Region focus
- **Click on a region name in the legend** — hide / show that region
- **Double-click on a region name in the legend** — show only that region, hide all others
- **Double-click again** — restore all regions

### Export
- **"Export PNG" button** — download a screenshot of the current view at high resolution (2×); the legend becomes opaque during capture
- **"Export 9 Region PNGs" button** — download 9 separate square images at 1900×1900 px, one per region; the selected region is highlighted with a glow effect, all others are shown dimly

## Files

| File | Description |
|------|-------------|
| `g25_coordinates.txt` | Source dataset — G25 coordinates across 25 principal components |
| `tda_mapper_clean.ipynb` | Jupyter notebook with the full pipeline |
| `index.html` | Interactive visualization (open in browser) |
| `g25_pca_scatter.png` | Standard PCA scatter for comparison |
| `k_selection.png` | K selection plots for K-means (elbow + silhouette) |

---

## Stack
python · pandas · numpy · scikit-learn · umap-learn · KeplerMapper

Visualization: matplotlib · scipy · Pillow · plotly · networkx · Figma page on Behance\
Interface: HTML · CSS · JavaScript · Plotly.js\
Support: Claude