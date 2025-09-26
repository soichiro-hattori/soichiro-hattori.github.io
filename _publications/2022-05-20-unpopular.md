---
title: "The unpopular Package: A Data-driven Approach to Detrending TESS Full-frame Image Light Curves"
collection: publications
category: manuscripts
# permalink: /publication/2025-06-05-ZTF-TESS
excerpt: "Soichiro Hattori, Daniel Foreman-Mackey, David W Hogg, Benjamin T Montet, Ruth Angus, TA Pritchard, Jason L Curtis, Bernhard Schölkopf"
date: 2022-05-20
venue: 'The Astronomical Journal'
paperurl: 'https://iopscience.iop.org/article/10.3847/1538-3881/ac625a/meta'
citation: 'Soichiro Hattori et al 2022 AJ 163 284'
---
The majority of observed pixels on the Transiting Exoplanet Survey Satellite (TESS) are delivered in the form of full-frame images (FFIs). However, the FFIs contain systematic effects such as pointing jitter and scattered light from the Earth and Moon that must be removed (i.e., “detrended”) before downstream analysis. We present unpopular, an open-source Python package to obtain detrended TESS FFI light curves optimized for variable sources. The unpopular package implements a variant of the causal pixel model to remove systematics and allows for simultaneous fitting with a polynomial component to capture nontransit astrophysical variations, such as supernova signals or stellar variability, that tend to be removed in techniques optimized for exoplanet detection. We validate our method by detrending different sources (e.g., supernovae, tidal disruption events (TDEs), exoplanet-hosting stars, fast-rotating stars) and comparing our light curves to those obtained by other pipelines when appropriate. Our supernova and TDE light curves are visually similar to those obtained by others using the ISIS image subtraction package, indicating that unpopular can be used to extract multisector light curves by preserving astrophysical signals on timescales of a TESS sector (∼27 days). We note that our method contains tuning parameters that are currently set heuristically, and that the optimal set of tuning parameters will likely depend on the particular signal the user is interested in obtaining. The unpopular source code and tutorials are freely available online.