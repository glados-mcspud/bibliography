# 'bibliografix'
# NOTE
# *** This is an active, first-time attempt at a full, albeit simple, program; the author is a proponent of open access and hopes that this mini-program, upon completion, will enable users to quantitatively scan and analyse their bibliographic data (_currently_ only from Web of Science), thus making scoping literature reviews much easier to conduct, at least in for the first instance of scoping. Its wide functionality is currently quite trivial as it is being used for a peer-reviewed publication, but the author intends to integrate user friendliness at the earliest convenience (i.e., upon completion of the manuscript in prep). For now, it is largely restricted to users of python, and more specifically, is written in Jupyter Notebook (.ipynb). The author hopes the current script (as it currently stands) will assist users, particularly those dealing with large datasets or perhaps even novel topics, with understanding what their raw bibliographic data says thus guiding them towards the most relevant literature for deep-diving into, e.g., certain materials and methods. ***   

# V0.1
This repository contains a python-based workflow for semi-automatically analysing bibliographic data—specifically data exported from Web of Science search queries. The project integrates Natural Language Processing (NLP), topic modeling (using Latent Dirichlet Allocation), clustering (using KMeans), and a suite of visualisation tools to help users explore and interpret their literature data. An interactive dashboard built with Streamlit will allow end users to "play around" with the data, filter records, and inspect topics visually upon completion of the script.

---

## Overview

The ultimate goal of this project is to take bibliographic export files (beginning with csv/Excel format(s) pending usefulness of the end product this will be expanded), clean and merge data, transform and preprocess textual information (combining article titles and abstracts), and then quantitatively analyse it using:
- **Topic Modeling:** LDA to extract latent topics within the literature.
- **Clustering:** KMeans for grouping similar documents (with quantitative distance metrics).
- **Visualisations:** For instance, word clouds, count plots, PCA scatter plots, bubble maps, geographical coverage, and more, to offer both an overview and detailed inspection of the dataset.
- **Interactive Dashboard:** The end goal will be to incorporate Streamlit functionalities to allow non-technical users to interact with and analyse the bibliographic data with adjustable parameters.

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

## Installation (Not currently recommended, though data being actively used by the author _is_ provided in its entirety and thereby transparently) 

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/glados-mcspud/bibliography.git
   cd bibliography.git
