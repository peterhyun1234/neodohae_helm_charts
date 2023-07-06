# neodohae_helm_charts

This repository contains Helm charts for the neodohae applications.

## Structure

The repository is structured as follows:

- `neodohae`: The root directory of the Helm chart
  - `Chart.yaml`: This file contains the metadata of the Helm chart
  - `values.yaml`: This file defines the default configuration values
  - `templates`: This directory contains the Kubernetes manifest files
    - `neodohae_common`: Contains common configurations
    - `neodohae_nestjs`: Contains configurations for the neodohae_nestjs application
    - `neodohae_nextjs`: Contains configurations for the neodohae_nextjs application

## Usage

To deploy the chart to your Kubernetes cluster, you can use the following commands:

```bash
helm repo add neodohae https://github.com/peterhyun1234/neodohae_helm_charts
helm install my-release neodohae
