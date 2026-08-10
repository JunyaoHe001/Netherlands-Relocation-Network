# Netherlands Relocation Network

This repository contains the public data, code, computational notebooks, documentation, and web resources for research on municipality-level population relocation networks in the Netherlands.

## Interactive atlas

The public atlas is available at:

**https://junyaohe001.github.io/Netherlands-Relocation-Network/atlas/**

It supports interactive filtering by year range and demographic stratum. Municipality colours represent net relocation balance, while directed curves represent the strongest origin–destination flows under the current selection.

The project landing page is available at:

**https://junyaohe001.github.io/Netherlands-Relocation-Network/**

## Dataset scope

The current data product covers annual inter-municipal relocation flows from **2011 to 2024**, harmonised to a common Dutch municipal geography and reconstructed for four demographic dimensions:

- age;
- sex;
- nationality;
- marital status.

The four dimensions are parallel marginal reconstructions. They should not be interpreted as a joint age × sex × nationality × marital-status cross-classification.

## Repository structure

```text
.
├── data/                 Public release files, metadata, and data documentation
├── docs/                 Methodological and project documentation
├── notebooks/            Versioned computational notebooks
├── outputs/              Reproducible figures, tables, and validation summaries
├── scripts/              Build, validation, and release utilities
├── src/                  Reusable analysis code
├── website/              Maintained project-page source and publication notes
└── gh-pages branch       Generated project website and interactive atlas
```

The `main` branch is reserved for research materials and maintained source files. Generated website assets are isolated on the `gh-pages` branch and served through GitHub Pages.

Large source or intermediate files should not be committed without a deliberate release strategy. Public, citable releases should be placed under `data/releases/` or attached to a versioned GitHub release, with checksums and metadata recorded in the repository.

## Reproducibility status

The repository is being populated in stages. The first stage establishes the publication structure and the interactive atlas. Subsequent releases will add the complete reconstruction workflow, analysis notebooks, data dictionaries, validation reports, and versioned public data packages.

## Citation

A provisional citation is:

> He, Junyao. *Dutch Municipality-Level Stratified Population Relocation Networks, 2011–2024*. Version 1.0. Netherlands Relocation Network repository.

A DOI-based citation will supersede this provisional citation after the first archived release.

## Licensing

- Code and website source: MIT License, unless a file states otherwise.
- Public data products: Creative Commons Attribution 4.0 International (CC BY 4.0), unless a release states otherwise.
- Third-party source data and map tiles remain subject to their original licences and attribution requirements.

## Contact

Junyao He  
J.HE@RUG.NL
