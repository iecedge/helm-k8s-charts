# helm-k8s-charts
helm-k8s-charts repo

This repo contains additional charts needed by SEBA and related applications, for arm64.
During installation of SEBA-in-a-Box, using automation-tools/seba-in-a-box/Makefile
(see https://gerrit.opencord.org/automation-tools.git) two helm repositories are referenced
as it results from 'helm repo list':
stable   	https://kubernetes-charts.storage.googleapis.com
incubator	https://kubernetes-charts-incubator.storage.googleapis.com/

Since these helm repos don't work at the moment for arm64 (no actual arm64 image), we will
host the modified charts in this repo, in a directory that corresponds to the name of the
helm repo referenced by SEBA-in-a-Box, i.e. stable and incubator.
