# Passbolt Helm chart for Kubernetes
Helm package for Passbolt project https://www.passbolt.com

## Installation

### 1. Using repo package
Add this helm repo:
```console
helm repo add passbolt https://gree-gorey.github.io/passbolt
helm repo update
```
Install passbolt:
```console
helm install passbolt/passbolt --name=my-passbolt-release
```

### 2. Using source github code
Clone/download source code:
```console
git clone https://github.com/gree-gorey/passbolt.git
```
Install passbolt:
```console
helm install ./passbolt --name=my-passbolt-release
```

## Configuration

The following table lists the configurable parameters of the Passbolt chart and their default values.

Parameter | Description | Default
--------- | ----------- | -------
`passbolt.persistence.size` | size of volume for `passbolt` pod | `5Gi`
`passbolt.ingress.host` | domain name for ingress resource | `example.com`
`mysql.persistence.size` | size of volume for `mysql` pod | `5Gi`
`mysql.rootPassword` | root password for `mysql`, plain | `secret`
`mysql.userPassword` | user password for `mysql`, plain | `secret`

See all available values in [values.yaml](https://github.com/gree-gorey/passbolt/blob/master/values.yaml)
