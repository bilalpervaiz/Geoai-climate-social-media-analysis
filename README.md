# GeoAI Analysis of Climate-Related Social Media Data

**Exploring climate discourse in Austria (2012–2023) through geospatial analysis, topic modelling, and emotion classification.**

This repository contains a Jupyter notebook used as a hands-on learning exercise at the **IEEE GRSS School on Earth Observation and GeoAI for Climate-Resilient Urban Systems**, held at **IT:U – Interdisciplinary Transformation University, Linz, Austria (14–16 October 2026)**.

The exercise demonstrates how location-associated social media posts can complement environmental and geospatial information by offering insights into public discussion and expressed emotions around climate-related issues.

## What the notebook covers

1. **Exploratory spatial and temporal analysis:** Load climate-related posts from Austria (2012–2023), explore their geographic distribution on interactive maps, and chart monthly posting activity.
2. **Topic modelling:** Use **BERTopic**, with **UMAP** for dimensionality reduction and **HDBSCAN** for clustering, to identify common themes in English- and German-language posts.
3. **Keyword-based exploration:** Filter posts by terms such as `klimakrise`, and inspect their spatial and temporal distribution.
4. **Emotion analysis:** Apply the multilingual transformer model [`MilaNLProc/xlm-emo-t`](https://huggingface.co/MilaNLProc/xlm-emo-t) to classify expressed emotions and explore their geographic and temporal patterns.
5. **Visualization:** Use **GeoPandas**, **Folium**, and **Plotly** to create maps and charts of climate-related discourse.

## Notebook

- [`GeoAI_and_climate_workshop.ipynb`](GeoAI_and_climate_workshop.ipynb)

## Getting started

The notebook is designed for **Google Colab**. Open it in Colab and execute the cells in order. A GPU runtime is recommended for the transformer-based steps.

The notebook installs some dependencies and downloads the prepared example dataset from a Google Drive link contained in the notebook. **Dataset availability and redistribution permissions are not guaranteed.** If the download is unavailable, an appropriately authorized dataset with matching fields will be needed.

The main Python packages used include `geopandas`, `pandas`, `bertopic`, `umap-learn`, `hdbscan`, `scikit-learn`, `transformers`, `nltk`, `folium`, `contextily`, `mapclassify`, `plotly`, and `wordcloud`.

> **Note:** Model outputs are estimates, not direct measurements of public opinion. Social media participation, geolocation, language, and emotion classification can introduce biases. The notebook is an educational demonstration, not a validated operational early-warning system.

## Credits and acknowledgement

**Original learning material:** This notebook was provided as part of the **IEEE GRSS School on Earth Observation and GeoAI for Climate-Resilient Urban Systems (2026)** at IT:U, Linz. Credit for the original workshop notebook, teaching approach, and supplied example dataset belongs to the **original workshop authors, instructors, and data providers**. This repository is shared for personal learning, practice, and educational reference; it does **not** claim original authorship of the workshop materials.

**School programme:** [IT:U – Earth Observation and GeoAI for Climate-Resilient Urban Systems](https://it-u.at/en/earth-observation-and-geoai-for-climate-resilient-urban-systems/#program)

**Acknowledgement:** Thank you to the school organizers, instructors, and IEEE GRSS community for the opportunity to learn and explore interdisciplinary GeoAI approaches to climate resilience.
