# Gaps and Overlaps Alpha Testing - ArcGIS Pro / ArcPy

## Overview

This notebook contains early prototype development and testing undertaken as part of the GEOM186 MSc GIS dissertation for ArcGIS Pro and ArcPy. The work explores automated ingestion of S-57 ENC data and identification of potential data coverage overlaps.

The prototype formed an initial proof of concept that later informed the development of the Gaps and Overlaps (GaOs) service.

## Contents

### S-57 Ingestion

The workflow imports S-57 ENC datasets (`*.000`) into an ArcGIS Maritime geodatabase using ArcPy and extracts Product Coverage (`M_COVR`) information for subsequent analysis.

### Overlap Analysis

The prototype performs spatial intersection analysis

Potential overlaps are filtered using IC-ENC policy rules based on navigational band and compilation scale.

### Automated Classification Experiments

Several approaches were tested for automatically classifying overlaps, including:

- Cartesian buffering.
- Ellipsoidal (geodesic) buffering.
- Distance-based categorisation of overlap geometries.

These experiments were used to evaluate whether overlap issues could be automatically prioritised before manual review.

## Status

This notebook represents exploratory alpha-phase development and contains experimental code, testing datasets, and alternative implementation approaches. It should be considered a research artefact rather than production software.