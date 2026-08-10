# Data

This directory is reserved for versioned public data products, metadata, dictionaries, validation summaries, and release manifests.

## Planned layout

```text
data/
├── metadata/              Variable dictionaries, group dictionaries, provenance, licences
├── samples/               Small examples suitable for testing and teaching
└── releases/
    └── v1.0.0/            Versioned public release package
```

The browser-ready JSON and GeoJSON files used by the interactive atlas are stored separately under `website/atlas/data/`. They are optimised for visualisation and should not be treated as a substitute for the complete analytical release.

## Core release units

The intended analytical release contains:

- directed municipality-to-municipality relocation flows by year and demographic group;
- calibrated municipality-level inflow and outflow margins;
- municipality and demographic-group dictionaries;
- municipal geography crosswalks and harmonisation metadata;
- reconstruction diagnostics and robustness summaries;
- checksums and a machine-readable manifest.

## Interpretation

Age, sex, nationality, and marital status are reconstructed as four parallel marginal network systems. Records from different demographic dimensions must not be combined as though they form a single joint cross-classified population table.

## File formats

Parquet is preferred for complete analytical tables. CSV may be supplied for dictionaries and summary tables. Each formal release should include a manifest recording relative path, file size, checksum, schema version, and release version.

## Licensing

Original public data products are released under CC BY 4.0 unless a release states otherwise. See [`LICENSE-DATA.md`](../LICENSE-DATA.md). Third-party inputs remain subject to their original terms.
