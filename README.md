# Federated Learning for Network Traffic Flow Classification

This is the supporting page for the manuscript titled, "*Network Traffic Flow Classification via Federated Learning*."

The paper presents a comparative study of Federated Learning models, developed under both IID and non-IID conditions, and a Centralized Learning model. The objective is to perform multi-class traffic flow classification for network applications.

In line with principles of reproducibility and transparency, and to support open science, the scripts utilized in the experiments are available to the public. Additionally, the dataset generated for this research is also accessible. These resources aim to aid a more comprehensive understanding of the methodologies employed and foster additional research in this field.

Researchers are encouraged to use this dataset for their investigations and to replicate or extend the findings of this study. The availability of this dataset is expected to support continued research in network flow analysis, thus adding to the body of knowledge in this area.

## Repository Structure

In our repository, the files and scripts are organized as follows:
 - [0-preliminaries.ipynb](0-preliminaries.ipynb) includes auxiliary functions needed for flow measurement and data preprocessing.
 - [1-prepare-datasets.ipynb](1-prepare-datasets.ipynb) houses the scripts for application label encoding, feature selection, and data set preparation for both centralized and federated learning models. Additionally, this file contains the code used to segment data into IID and non-IID chunks for federated learning. It also features scripts for visualizing data distribution across various application types, both for the full dataset and individual chunks.
 - [2-evaluate-cl.ipynb](2-evaluate-cl.ipynb) incorporates the code used to execute centralized learning and visualize the obtained results, which are stored as a JSON file at [results/cl_results.json](results/cl_results.json). In this file, you can see how the centralized model is trained and tested, and the process of result visualization.
 - [3-evaluate-fl-iid.ipynb](3-evaluate-fl-iid.ipynb) contains the functions employed for a visual comparison of Federated Learning (FL) results under IID conditions, stored at [results/fl_results.json](results/fl_results.json), against the centralized learning (CL) results found at [results/cl_results.json](results/cl_results.json). It offers a comparative analysis between FL (under IID conditions) and CL results.
 - [4-evaluate-fl-non-iid.ipynb](3-evaluate-fl-non-iid.ipynb) holds the functions used for visual comparison of FL results achieved under non-IID conditions, which are stored at [results/fl_results.json](results/fl_results.json), against the CL results found at [results/cl_results.json](results/cl_results.json). This notebook will helped to compare and understand the performance differences between FL (under non-IID conditions) and CL models.

The Jupyter notebooks are designed to be self-explanatory, guiding the reader through each step of the process. However, if any issues are encountered or something is unclear, it is encouraged to raise an issue on GitHub. Contributions to the improvement of this repository are greatly appreciated.

## Federated Learning

The FL models incorporated in the study were constructed utilizing our [FeNOMan framework](https://www.nfstream.org/fenoman.github.io/). This framework played a crucial role in the development and optimization of the FL models. Researchers can refer to the FeNOMan documentation for a comprehensive understanding of the functions and capabilities it offers.

## Dataset

The dataset necessary to execute these notebooks are available at [datasets/dataset.zip](datasets/dataset.zip). Exploration and use of these datasets for research purposes is strongly encouraged.

## Documentation

For a deeper understanding of the project, reference can be made to the related research paper. There, additional insights about the methodologies employed can be found.

We hope this repository serves as a valuable resource in related research.



