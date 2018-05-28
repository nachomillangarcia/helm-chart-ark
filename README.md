# HEPTIO ARK

Chart to deploy [Heptio Ark](https://github.com/heptio/ark) backups solutions. It comes preconfigured for AWS S3 backend but that's easily customizable.

## Installing the Chart
```
helm install --name my-heptio-ark .
```

## Configuration

The following table lists the configurable parameters of the heptio-ark chart and their default values.

s3Bucket: my-s3-ark-bucket
AWS_AK: ACCESSKEY
AWS_SK: SECRETKEY
arkNamespace: heptio-ark

| Parameter | Description | Rquired | Default |
| --------- | ----------- | ------- | ------- |
| `s3Bucket` | S3 Bucket name | yes | |
| `AWS_AK` | AWS Access Key | yes | |
| `AWS_SK` | AWS Secret Key | yes | |
| `arkNamespace` | Namespace to store backups | yes | heptio-ark |

## Other Charts
This chart is based in [this PR](https://github.com/kubernetes/charts/pull/3795) in the official charts repository (open at the moment).
