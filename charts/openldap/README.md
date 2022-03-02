# openldap

![Version: 0.3.0](https://img.shields.io/badge/Version-0.3.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 2.4.59](https://img.shields.io/badge/AppVersion-2.4.59-informational?style=flat-square)

A Helm Chart to deploy openLDAP in Kubernetes, using the openSUSE openLDAP image

## TL;DR
```console
$ helm repo add johanneskastl-openldap https://johanneskastl.github.io/openldap-helm-chart/
$ helm repo update
$ helm install openldap johanneskastl/openldap
```

## Installing the Chart
To install the chart with the release name `openldap`:
```console
helm install openldap johanneskastl/openldap
```

## Uninstalling the Chart
To uninstall the `openldap` deployment:
```console
helm uninstall openldap
```
The command removes all the Kubernetes components associated with the chart and deletes the release.

## Configuration

Read through the [values.yaml](./values.yaml) file. It has several commented out suggested values.

Specify each parameter using the `--set key=value[,key=value]` argument to `helm install`. For example,
```console
helm install openldap \
  --set env.TZ="America/New York" \
    johanneskastl/openldap
```

Alternatively, a YAML file that specifies the values for the above parameters can be provided while installing the chart.
For example,
```console
helm install openldap johanneskastl/openldap -f values.yaml
```

