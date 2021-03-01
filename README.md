# application-chart
Open Cluster Management Application console Helm chart

------

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [Getting Started](#getting-started)
- [Prerequisite Tools](#prerequisite-tools)
- [Building for Development](#building-for-development)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

------

## Getting Started
Application chart is a helm chart used for deploying the [Application console](https://github.com/open-cluster-management/application-ui). This is a guide on how to build and run open-cluster-management application-chart.

## Prerequisite Tools

- [helm](https://helm.sh/docs/intro/install/)

## Building for Development
<pre>
git clone https://github.com/open-cluster-management/application-chart.git
cd application-chart
helm package stable/application-chart
</pre>
