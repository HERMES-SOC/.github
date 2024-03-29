Welcome to the Heliophysics Environmental and Radiation Measurement Experiment Suite (HERMES) Science Operations Center (SOC) codebase.
This project is part of the [Space Weather Science Operations Center (SWxSOC)](https://swxsoc.github.io). It makes use of the NASA Science Managed Cloud Environment ([SMCE](https://smce.nasa.gov)). This set of repositories is responsive to the new [NASA SMD Heliophysics (HPD) Data Policy](https://science.nasa.gov/science-red/s3fs-public/atoms/files/HPD_Data_Policy_Final_20220209_TAGGED.pdf) requirement that 
  * HPD-funded software shall be released under a permissive license that has
broad acceptance in the community and shall be made available in a publicly
accessible repository that is widely recognized by the community. If
commercial software is used, then the HPD-funded executable code shall be
released and made available.

## Code of Conduct

Interactions in this community are governed by
our [Code of Conduct](https://github.com/HERMES-SOC/code-of-conduct/blob/main/CODE_OF_CONDUCT.md).

## Repository Index

### Project Documentation
* **[hermes-pdmp](https://github.com/HERMES-SOC/hermes-pdmp)**: The project data management plan.

### Science Processing and Data Analysis
* **[hermes_core](https://github.com/HERMES-SOC/hermes_core)**: A central Python Package for common functionality across all hermes instruments
* **[hermes_instrument](https://github.com/HERMES-SOC/hermes_instrument)**: A Python package template for the instrument packages.
* **[hermes_eea](https://github.com/HERMES-SOC/hermes_eea)**: A Python package to process and analyze data from the HERMES EEA instrument.
* **[hermes_merit](https://github.com/HERMES-SOC/hermes_merit)**: A Python package to process and analyze data from the HERMES MERIT instrument.
* **[hermes_nemisis](https://github.com/HERMES-SOC/hermes_nemisis)**: A Python package to process and analyze data from the HERMES NEMISIS instrument.
* **[hermes_spani](https://github.com/HERMES-SOC/hermes_spani)**: A Python package to process and analyze data from the HERMES SPAN-I instrument.

### AWS Pipeline Architecture, Code, and Support
* **[sdc_aws_pipeline_architecture](https://github.com/HERMES-SOC/sdc_aws_pipeline_architecture)**: AWS CDK code for the file processing pipeline architecture
* **[sdc_aws_sorting_lambda](https://github.com/HERMES-SOC/sdc_aws_sorting_lambda)**: AWS Lambda code for sorting files into the instrument buckets
* **[sdc_aws_processing_lambda](https://github.com/HERMES-SOC/sdc_aws_processing_lambda)**: AWS Lambda code for processing files in the instrument buckets
* **[sdc_aws_base_docker_image](https://github.com/HERMES-SOC/sdc_aws_base_docker_image)**: Docker image for the base image for the processing Lambda/Development containers
* **[CDFTracker](https://github.com/HERMES-SOC/CDFTracker)**: A python package that helps track Raw Binary and CDF Files in a Relational Database
* **[FSWatcher](https://github.com/HERMES-SOC/sdc_aws_fswatcher)**: A filewatcher system that can be configured to watch a directory for new files and then upload them to an S3 bucket.
* **[S3Watcher](https://github.com/HERMES-SOC/sdc_aws_s3watcher)**: A filewatcher system that can be configured to watch an AWS S3 bucket new files and then download them onto a local machine.
* **[sdc_aws_grafana_dashboard_backups](https://github.com/HERMES-SOC/sdc_aws_grafana_dashboard_backups)** : Backs up deployed dashboards as JSON models on https://grafana.hermes.swsoc.smce.nasa.gov/ daily

## Presentations and Publications
* [DASH 2023](https://dash.heliophysics.net), Robbertz, Andrew, Rager, Amy C., Barrous-Dume, Damian, Skeberdis, Daniel, Christe, Steven, Kreisler, Steve, Mercer, Tony, & Paterson, William R. (2023). The Architecture and Functionality of HERMES Core and Instrument Python Packages. Zenodo. [https://doi.org/10.5281/zenodo.8400671](https://doi.org/10.5281/zenodo.8400671)
* [DASH 2023](https://dash.heliophysics.net), Damian Barrous-Dume, Amy Catherine Rager, Andrew Robbertz, Daniel Skeberdis, Steven Christe, Steve Kreisler, Tony Mercer, & William R Paterson. (2023, October 9). Open Science in Action: SWxSOC's Role in Accelerating Data Release and Cloud Processing for Heliophysics Missions. Zenodo. [https://doi.org/10.5281/zenodo.8408028](https://doi.org/10.5281/zenodo.8408028)

