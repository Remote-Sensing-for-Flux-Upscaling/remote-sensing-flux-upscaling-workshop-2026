# Remote Sensing and Fluxes Upscaling for Real-world Impact: Integration with Advanced Techniques” workshop (March 2026) NEEDS TO BE UPDATED

## Introduction

The 2026 workshop built directly on the 2024 Berkeley meeting and shifted the series from conceptual articulation toward operational practice. The proposal emphasized five linked objectives: evaluating scalable flux-integration frameworks, strengthening scale matching in heterogeneous landscapes, training early-career scientists in open and cloud-based tools, bridging science with applications, and catalyzing cross-sector collaboration. 

## 2026 Remote Sensing and Fluxes Upscaling for Real-world Impact workshop
This repository contains materials from the 2026 Remote Sensing and Fluxes Upscaling for Real-world Impact workshop focused on analyzing and integrating remote sensing and flux data using Jupyter Notebooks. The workshop featured a series of presentations, which are outlined in the agenda included in this repository. 

The repository is organized as follows:
- **Hands-on Tutorial**: A collection of Jupyter notebooks providing tutorials and examples for working with remote sensing and flux data, designed to be run on Google Colab.
- **Presentations**: The workshop presentations, including slides and supporting materials, are presented in accordance with the agenda. The available slides are from speakers who have granted permission to make their material publicly available. 

To run the notebooks, simply open them in Google Colab and follow the instructions. This repository aims to provide a resource for participants and others interested in learning about remote sensing and flux data analysis and integration.

### External Resorces 
- Workshop report [here]()
- Datasets created and used in the hands-on session can be found [here]((https://drive.google.com/drive/folders/1OvxaLGMslmKTExFAZ1rs4xiznROQW4k5?usp=sharing).
- Recordings of the sessions are available on the [event] page .  

## Workshop PIs

## Workshop Organizing Committee
Adam Young (National Ecological Observatory Network)  
Chris Florian (National Ecological Observatory Network) 
David Durden (National Ecological Observatory Network)  
David Moore (The university of Arizona)
Housen Chu (Lawrence Berkeley National Laboratory - AmeriFlux Management Project)  
Leila Hernandez-Rodriguez (Lawrence Berkeley National Laboratory)  
Nicola Falco (Lawrence Berkeley National Laboratory - AmeriFlux Management Project)  
Samuel Bower (AtmoFacts, Carbon Dew Community of Practice)  
Stefan Metzger (AtmoFacts, Carbon Dew Community of Practice)  
Yanghui Kang (Virginia Tech)

### Coordinator
David Durden (National Ecological Observatory Network)  


## Hands-on Tutorial
### Topic 1: From site-scale ...   
Creators: Nicola Falco (nicolafalco@lbl.gov), David Durden (ddurden@battelleecology.org), Stefan Metzger (smetzger@atmofacts.com)  

This topic focuses on site-scale analysis using remote sensing (RS) data:
- How to collect RS data using Google Earth Engine (GEE) and Colab (Python API)
- How to process the data using practical codes, covering key steps such as:
    - Calculating vegetation indices
    - Visualizing data as maps
    - Extracting time-series information
    - Conducting quality assessment (QA)
    - Comparing RS time-series with tower flux data (Net Ecosystem Exchange, NEE)
    - Aggregating RS and flux time-series data
    - Modeling the relationship between vegetation indices and NEE using a linear model.

### Topic 2: ... over regional-scale connectivity ...
Creators: Nicola Falco (nicolafalco@lbl.gov), David Durden (ddurden@battelleecology.org), Stefan Metzger (smetzger@atmofacts.com)  

In Topic 2 of this tutorial, we explore regional-scale connectivity by:
- Applying the linear model developed in Topic 1 to estimate Net Ecosystem Exchange (NEE) over a small region, using a straightforward analysis approach
- Utilizing high-frequency flux spatialization to investigate additional factors influencing NEE in space, time, and process.

### Topic 3: ... to continental-scale connectivity
Creators: Danielle Losos (losos@wisc.edu), Paul Stoy (pcstoy@wisc.edu), Avanti Kekane (avkekane@wisc.edu), Sophie Hoffman (shoffman22@wisc.edu), Sadegh Ranjbar (sranjbar@wisc.edu), Ryan Abernathey (ryan@earthmover.io)  

In Topic 3, we scale up to continental connectivity by introducing the Advanced Baseline Imager Live Imaging of Vegetated Ecosystems ([ALIVE](https://alive-abi.github.io/alive/index.html)) workflow that we call 'ALIVE<sub>GPP</sub>', also described in this [google slides presentation](https://docs.google.com/presentation/d/1PJclqluGFHkp9LpHZ85_pgL8lFLLaAMsQcEGZ2DIGSU/edit#slide=id.p1) that was created for the workshop. The tutorial covers:
- How to work with [zarr](https://zarr.dev/) libraries created using [Icechunk](https://icechunk.io/en/latest/overview/#docs-organization) by [earthmover](https://earthmover.io/). We will use a zarr library that contains [Gross Primary Productivity (GPP) estimates](https://alive-abi.github.io/alive/daily-GPP.html) from the ALIVE worksflow.
- Leveraging data from the [Advanced Baseline Imager](https://www.goes-r.gov/spacesegment/abi.html) on the [Geostationary Operational Environmental Satellites - R Series (GOES-R)](https://www.goes-r.gov/) to create ALIVE<sub>GPP</sub> for pixels that contain Ameriflux and NEON, Inc. towers as described in [Losos et al. (2024)](https://www.nature.com/articles/s41597-024-03071-z)
- Using a machine learning model specifically a gradient boosting model described in [Ranjbar et al. (2024)](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2024MS004341), to estimate GPP at the native temporal resolution of the ABI CONUS scene, every 5 minutes, as described in [Losos et al. (2025)](https://www.sciencedirect.com/science/article/pii/S0034425725001634).

## Acknowledgments
### Workshop report
If you use any of the content discussed in the workshop report or tutorial, please cite the following document.
- Falco, Nicola, Durden, David, Metzger, Stefan, Stoy, Paul, Yi, Koong, Florian, Chris, & Barnes, Mallory (2024). Workshop Report: Remote Sensing and Fluxes Upscaling for Real-world Impact. https://doi.org/10.2172/3001093

### Hands-on Tutorial
This tutorial was developed using resources and data from various sources. If you use this tutorial or modify it for your own research or educational purposes, please acknowledge the original repository and contributors.

To acknowledge this repository, please cite it as follows:

#### Topics 1 & 2:
- Falco, Nicola, Metzger, Stefan, and Durden, David, "2024 Workshop - Remote Sensing and Fluxes Upscaling for Real-world Impact - Tutorial v1," (2025), https://doi.org/10.11578/dc.20251024.5

#### Topic 3:
- Losos, D., Hoffman, S. & Stoy, P.C. GOES-R land surface products at Western Hemisphere eddy covariance tower locations. Sci Data 11, 277 (2024). https://doi.org/10.1038/s41597-024-03071-z
- Ranjbar, S., Losos, D., Hoffman, S., Cuntz, M., & Stoy, P. C. (2024). Using geostationary satellite observations and machine learning models to estimate ecosystem carbon uptake and respiration at half hourly time steps at eddy covariance sites. Journal of Advances in Modeling Earth Systems, 16, e2024MS004341. https://doi.org/10.1029/2024MS004341
- Losos, D., Ranjbar, S., Hoffman, S., Abernathey, R., Desai, A. R., Otkin, J., Zhang, H., Ryu, Y., & Stoy, P. C. (2025). Rapid changes in terrestrial carbon dioxide uptake captured in near-real time from a geostationary satellite: The ALIVE framework. Remote Sensing of Environment, 324, 114759. https://doi.org/10.1016/j.rse.2025.114759

By acknowledging this repository and its contributors, you help to promote transparency, reproducibility, and recognition of the work that has gone into creating this resource.

## License
See [License](https://github.com/Remote-Sensing-for-Flux-Upscaling/remote-sensing-flux-upscaling-workshop-2026/edit/main/README.md#:~:text=Presentations-,LICENSE,-README.md) file for licensing.

## Funding acknowledgements
NSF Award 2532339 “Conference: Remote Sensing and Fluxes for Real-world Impact: Integration with Advanced Techniques”
PIs (David Durden (Battelle – NEON); Stefan Metzger (AtmoFacts); Nicola Falco (LBNL – AMP))
