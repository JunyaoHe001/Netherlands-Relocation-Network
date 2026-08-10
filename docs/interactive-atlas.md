# Interactive atlas: data and visual interpretation

## Purpose

The interactive atlas presents annual municipality-level relocation networks for the Netherlands by demographic stratum. It is a public exploration layer for the research dataset and is not intended to replace the complete analytical release.

## Controls

The interface provides:

- a two-handle year-range selector;
- annual-average and period-total aggregation;
- a demographic-dimension selector;
- group-level checkboxes within the selected dimension;
- a municipality search function;
- a configurable upper limit for displayed origin–destination edges;
- downloadable node and displayed-edge summaries for the current selection.

## Node colours

Municipality colours represent net relocation balance:

```text
net flow = inflow − outflow
```

Negative values indicate net outflow and positive values indicate net inflow. The diverging colour scale is centred at zero. To prevent a small number of extreme municipalities from compressing the colour variation elsewhere, the display range is clipped symmetrically using the configured quantile of absolute net-flow values.

Node inflows, outflows, and net flows are calculated from the complete calibrated municipality margins for the selected years and groups.

## Network edges

Directed curves represent origin–destination relocation flows. For browser performance, the public build retains the strongest candidate edges independently for each year and demographic group. The interface then ranks the aggregated candidates under the current filter and displays the requested number of strongest edges.

The atlas reports candidate and visible-flow coverage. Displayed edges are therefore a documented visualisation layer, while node balances are based on complete margins.

## Demographic dimensions

Age, sex, nationality, and marital status are separate marginal reconstructions. Multiple groups may be aggregated within one dimension. Groups from different dimensions cannot be interpreted as intersections or added together without double counting the same underlying total network.

## Geography

Municipal records are harmonised to a common geography for longitudinal comparison. Public geometry is simplified for browser rendering, while municipality identifiers and names are retained in the release metadata.

## Reproducibility

The atlas is generated from the versioned STEP5 notebook under `notebooks/05_publication/`. Build reports include source-contract information, source-notebook version, asset checksums, geometry source, edge-retention settings, and coverage summaries.
