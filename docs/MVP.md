An MVP for this extension is a `nifti_metadata(...)` function that (using DuckDB) returns a table with the metadata of a [nifti](https://nifti.nimh.nih.gov/) file.

Nifti 1 is a more stable format than Nifti 2, so this is the most natural choice. Documentation for the nifti 1 format is available [here](https://nifti.nimh.nih.gov/nifti-1).

This is relatively similar to the `parquet_metadata` function in the base duckdb parquet [extension](https://github.com/duckdb/duckdb/blob/master/extension/parquet/parquet_metadata.cpp).
