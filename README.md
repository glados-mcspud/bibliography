# bibliography
Semi-automation of bibliographic data/information sourced from Web of Science

This repository contains a Python-based workflow for semi-automatically analyzing bibliographic data—specifically data exported from Web of Science search queries. The project integrates Natural Language Processing (NLP), topic modeling (using Latent 
Dirichlet Allocation), clustering (using KMeans), and a suite of visualization tools to help users explore and interpret their literature data. An interactive dashboard built with Streamlit allows end users to "play around" with the data, filter records, 
and inspect topics visually.

---

## Overview

The goal of this project is to take bibliographic export files (in Excel format), clean and merge the data, transform and preprocess textual information (combining article titles and abstracts), and then analyse it using:
- **Topic Modeling:** Using LDA to extract latent topics within the literature.
- **Clustering:** Using KMeans for grouping similar documents (with quantitative distance metrics).
- **Visualisations:** Including word clouds, count plots, PCA scatter plots, bubble maps, and more to offer both an overview and detailed inspection of the dataset.
- **Interactive Dashboard:** A prototype built using Streamlit allows non-technical users to interact with and analyze the bibliographic data with adjustable parameters.

This pipeline is intended to be open, reproducible, and extensible for researchers looking to gain meaningful insights from their literature collections.

---

## Features

- **Data Loading & Merging:** Automatically detect and merge multiple Excel files exported from Web of Science.
- **Data Cleaning & Filtering:** Remove duplicate entries, filter non-journal or non-English records, and drop empty columns.
- **Text Preprocessing:** Combine article titles and abstracts into a single field to preserve context.
- **Topic Modeling (LDA):** Identify latent topics from the text data, assign a dominant topic and confidence weight for each document.
- **KMeans Clustering:** Group documents based on textual similarity and compute distance measures that highlight representative documents.
- **Variety of Visualizations:**  
  - Count plots and bar charts for journal and category distributions.  
  - PCA scatter plots for visualizing clusters of documents.  
  - Word clouds from article titles.  
  - Bubble maps of geographical data using Plotly Express.
- **Interactive Dashboard (in progress):** A Streamlit-based dashboard enabling users to filter bibliographic data by language, topic, or other criteria and see interactive visualizations.

---

## Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/glados-mcspud/bibliography.git
   cd bibliography.git
