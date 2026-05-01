# 2nd Workshop: "Remote Sensing and Fluxes Upscaling for Real-world Impact: Integration with Advanced Techniques” (March 2026) 

## Introduction

The 2026 workshop built directly on the 2024 Berkeley meeting and shifted the series from conceptual articulation toward operational practice. The workshop emphasized five linked objectives: evaluating scalable flux-integration frameworks, strengthening scale matching in heterogeneous landscapes, training early-career scientists in open and cloud-based tools, bridging science with applications, and catalyzing cross-sector collaboration. The workshop convened the remote sensing, flux, AI, and applications communities in Boulder on 4–5 March 2026. Across two days, the meeting moved from conceptual framing and hands-on tutorials to application talks, a career roundtable, posters, fluxART installations, and collaborative group projects. The workshop’s strongest unifying idea was that flux upscaling should be approached as a deliberate nesting problem—that is, combining complementary methods across scales rather than relying on a single universal model. Spatialized eddy covariance emerged as the preferred measurement anchor. Multi‑time, multi‑site learning helped extend regional coverage. Knowledge‑guided machine learning improved the stability of extrapolations. Foundation models provided broader, but more abstract, forms of inference. 

## This Repository
This repository contains materials from the 2026 Remote Sensing and Fluxes Upscaling for Real-world Impact workshop focused on analyzing and integrating remote sensing and flux data using Jupyter Notebooks. The workshop featured a series of presentations, which are outlined in the agenda included in this repository. 

The repository is organized as follows:
- **Hands-on Tutorial**: A collection of Jupyter notebooks providing tutorials and examples for working with remote sensing and flux data, designed to be run on Google Colab.
- **Presentations**: The workshop presentations, including slides and supporting materials, are presented in accordance with the agenda. The available slides are from speakers who have granted permission to make their material publicly available. 

To run the notebooks, simply open them in Google Colab and follow the instructions. This repository aims to provide a resource for participants and others interested in learning about remote sensing and flux data analysis and integration.

### External Resorces 
- [Workshop report](https://zenodo.org/badge/DOI/10.5281/zenodo.19767226.svg)

- Posters can be found on our [Zenodo comunity page](https://zenodo.org/communities/remote-sensing-and-flux-upscaling-community/records?q=&l=list&p=1&s=10&sort=newest)
- [Datasets](https://drive.google.com/drive/folders/1OvxaLGMslmKTExFAZ1rs4xiznROQW4k5?usp=sharing) created and used in the hands-on session.
- Recordings of the sessions [TBD]

## Workshop Organizing Committee
David Durden (National Ecological Observatory Network, Battelle)  
Nicola Falco (Lawrence Berkeley National Laboratory - AmeriFlux Management Project)  
Stefan Metzger (AtmoFacts, Carbon Dew Community of Practice)   
Adam Young (National Ecological Observatory Network)  
Chris Florian (National Ecological Observatory Network)  
David Moore (The university of Arizona)  
Housen Chu (Lawrence Berkeley National Laboratory - AmeriFlux Management Project)   
Leila Hernandez-Rodriguez (Lawrence Berkeley National Laboratory)   
Samuel Bower (AtmoFacts, Carbon Dew Community of Practice)   
Yanghui Kang (Virginia Tech)   

### Coordinator
David Durden (National Ecological Observatory Network, Battelle)  


## Hands-on Tutorial
### Topic 1: Introduction to Remote Sensing Data Gathering  
#### GEE data gathering
This tutorial provides an introduction to using Colab notebooks with Google Earth Engine Python library to gather and process remote sensing (RS) data:
- How to collect RS data using Google Earth Engine (GEE) and Colab (Python API)
- How to process the data using practical codes, covering key steps such as:
    - Calculating vegetation indices
    - Visualizing data as maps
    - Extracting time-series information
    - Conducting quality assessment (QA)
    - Visualize hyperspectral and LiDAR data from acquired by NEON AOP

#### Reading public ALIVE data
This tutorial provides an introduction to the Advanced Baseline Imager Live Imaging of Vegetated Ecosystems (ALIVE) workflow and the use of zarr libraries created using Icechunk by earthmover, which allows for cloud-optimized geospatial processing. ALIVE provides estimates of carbon fluxes in real time using geostationary "weather" satellites, especially GOES-R (the Geostationary Operational Environmental Satellite - R Series). To learn more about ALIVE, visit their [GitHub page](https://alive-abi.github.io/alive/index.html).

### Topic 2: Interfacing flux Scaling Approaches Across Space and Time
This tutorial will investigate datasets from the BenchFlux working group (www.benchflux.org) to see how different approaches ranging from direct flux observations to global knowledge-guided models capture NEE fluxes.

### Topic 3: Exploring AI Foundation Model Techniques for Carbon Flux Prediction
This tutorial provides hands-on experience in using large-scale Earth Observation foundation models for GPP prediction and benchmarking their performance against classical machine learning approaches. Specifically, participants will:
- Integrate 30m HLS imagery with 10 MERRA atmospheric variables
- Fine-tune Prithvi-EO-2.0-300M-TL and Prithvi-EO-2.0-600M-TL for GPP prediction
- Train Random Forest and XGBoost models on the same dataset
- Evaluate predictive performance using the coefficient of determination (R²)
- Compare the impact of model scale (300M vs 600M) and architecture type (foundation vs tree-based)

## Acknowledgments
### Workshop report and tutorial
This tutorial was developed using resources and data from various sources. If you use this tutorial or modify it for your own research or educational purposes, please acknowledge the original (this) repository and contributors. If you use any of the content discussed in the workshop report or hands-on tutorial, please cite the following document. This material is based in part upon work supported by the National Ecological Observatory Network (NEON), a program sponsored by the U.S. National Science Foundation (NSF) and operated under cooperative agreement by Battelle.
- report citation to be added

### Funding
NSF Award 2532339 “Conference: Remote Sensing and Fluxes for Real-world Impact: Integration with Advanced Techniques”
PIs (David Durden (Battelle – NEON); Stefan Metzger (AtmoFacts); Nicola Falco (LBNL – AMP))

By acknowledging this repository and its contributors, you help to promote transparency, reproducibility, and recognition of the work that has gone into creating this resource.

## License
See [License](https://github.com/Remote-Sensing-for-Flux-Upscaling/remote-sensing-flux-upscaling-workshop-2026/edit/main/README.md#:~:text=Presentations-,LICENSE,-README.md).


