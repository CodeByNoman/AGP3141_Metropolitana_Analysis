# 🌿 Urban Green Space Visualization in Metropolitan Chile

This project visualizes urban population distribution and green space availability per inhabitant across communes in the Metropolitan Region of Chile. It combines spatial data with statistical summaries to produce thematic maps and bar charts using R.

## 📦 Project Structure
```
├── AGP3141_Metropolitana_Analysis/
│   ├── datos/
│   │   ├── metropolitana.geojson                 # Spatial boundaries of communes
│   │   └── areaverde_por_habitante.csv           # Green area per inhabitant data
│   ├── figures/
│   │   ├── urban_population_map.png              # Output map showing urban population
│   │   └── green_area_bar_chart.png              # Output chart showing green area per inhabitant
│   ├── main.R                                    # Main R script for analysis and visualization
│   └── README.md                                 # Project documentation
```
## 📊 Visualizations

- **Thematic Map**: Displays urban population density using a quantile-based color scale, with additional cartographic elements like compass, scale bar, and minimap.
- **Bar Chart**: Shows median green area per inhabitant by commune, with clear labels and a horizontal legend.

## 🛠️ Technologies Used

- **R** with the following packages:
  - `sf` – for handling spatial vector data
  - `tmap` – for thematic mapping
  - `tidyverse` – for data manipulation and plotting
  - `janitor` – for cleaning column names
  - `ggplot2` – for bar chart visualization
  - `patchwork` – for combining plots

## 📂 Data Sources

- `metropolitana.geojson`: Spatial boundaries of communes.
- `areaverde_por_habitante.csv`: Green area per inhabitant statistics.

## 📌 Key Features

- Clean and consistent data joining using `janitor::clean_names()`.
- Population labels formatted as short numbers (e.g., "1.2M", "850k").
- Custom map layout with serif fonts and bold legend titles.
- Bar chart with reordered communes and rounded labels.

## 👤 Author

**Noman Ahmad**  
Date: 2025-10-31  
CRS: EPSG:4326

## 📖 Reference

This project makes extensive use of the **tmap** package for spatial visualization. For a comprehensive guide, refer to:

> Tennekes M., Nowosad J. (2025) *Spatial Data Visualization with tmap: A Practical Guide to Thematic Mapping in R*. Available at: https://tmap.geocompx.org
