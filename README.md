> This repository has been deprecated in ACM 2.6.z and later. It has been moved to <https://github.com/stolostron/multiclusterhub-operator> as a sub-package `pkg/templates/charts/toggle/console`.

# application-chart
Open Cluster Management Application console Helm chart

------

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [application-chart](#application-chart)
  - [Work in Progress](#work-in-progress)
  - [Community, discussion, contribution, and support](#community-discussion-contribution-and-support)
  - [Getting Started](#getting-started)
  - [Prerequisite Tools](#prerequisite-tools)
  - [Building for Development](#building-for-development)
  - [Testing on an existing OKD cluster with OCM](#testing-on-an-existing-okd-cluster-with-ocm)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

------

## Work in Progress

 We are in the process of enabling this repo for community contribution. See wiki [here](https://open-cluster-management.io/concepts/architecture/).

## Community, discussion, contribution, and support

Check the [CONTRIBUTING Doc](CONTRIBUTING.md) for how to contribute to the repo.

## Getting Started

Application chart is a helm chart used for deploying the [Application console](https://github.com/stolostron/application-ui). This is a guide on how to build and run stolostron application-chart.

## Prerequisite Tools

- [helm](https://helm.sh/docs/intro/install/)

## Building for Development

```bash
git clone https://github.com/stolostron/application-chart.git
cd application-chart
helm package stable/application-chart
```

## Testing on an existing OKD cluster with OCM

Make sure you are logged in using `oc`.

```bash
export GITHUB_TOKEN=&lt;your github personal access token&gt;
export GITHUB_USER=&lt;your github id&gt;
cd ..
git clone https://github.com/stolostron/multiclusterhub-repo.git
cd application-chart
cp application-chart-&lt;version&gt;.tgz ../multiclusterhub-repo/multiclusterhub/charts
cd ../multiclusterhub-repo
oc annotate mch multiclusterhub -n open-cluster-management mch-pause=true
make update-charts
oc annotate mch multiclusterhub -n open-cluster-management mch-pause=false --overwrite
```
