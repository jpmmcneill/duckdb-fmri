## What is fMRI data

[fMRI](https://en.wikipedia.org/wiki/Functional_magnetic_resonance_imaging) (functional MRI) is a subset of MRI imaging that is typically used for analysing brains.

Analysis of fMRI data is typically done in Python, using packages such as [NiPy](https://nipy.org/). This organisation has several open source [projects](https://github.com/nipy) focusing on (f)MRI data.

There are several common problems involved with fMRI data. A few examples are given:
- Brain normalization. Each person's brain is a slightly different size, and as such renormalizing sizes to a "template" is often applied to facilitate cross brain comparisons.
- Motion correction. During scans, peoples heads can move (and some heads move more than others).

## Why DuckDB?

The data volume of fMRI (particularly in scientific circles, where scans last up to 30 mins or more) can become quite large. In memory analytics with python packages can be slow.

DuckDB (particularly it's vectorized engine) has solved these types of problems countless times. Lower analysis run times means that Doctors and Scientists can spend more time on the things that really matter, rather than simply waiting for code to run.

This project is not super likely to be useful (at least in the short term), as I am using it as a strong refresher to my cpp knowledge. Suggestions and / or contributions are welcome!

I am also looking for labs / hospitals who have experienced the above outlined problems. I am loosely familiar with the trinity [Cusack Lab](https://www.cusacklab.org/) which will hopefully give some insight into problems that exist in this space. 

## Roadmap

This extension to [DuckDB](https://duckdb.org/)

- Finalise extension goals
- Ability to parse MRI data files into duckdb
- Support of typical transformation / analytical functions performed using sql
