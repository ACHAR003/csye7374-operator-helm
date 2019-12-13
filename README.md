# CSYE7364 Operator Helm Chart

* Installs the s3 operator

## TL;DR;

```console
$ helm install csye7374-operator-helm
```

## Installing the Chart

To install the chart with the release name `my-release`:

```console
$ helm install csye7374-operator-helm/ --set operator.accessKey="AWS_ACCESS_KEY" --set operator.secrtAccessKey="AWS-SECRET-ACCESS-KEY" --set operator.bucketName="BUCKET-NAME" --set operator.image="OPERATOR-IMAGE" 
```

## Uninstalling the Chart

To uninstall/delete the my-release deployment:

```console
$ helm del my-release --purge
```

The command removes all the Kubernetes components associated with the chart and deletes the release.

## Configuration

| Parameter                                 | Description                                   | Default                                                 |
|-------------------------------------------|-----------------------------------------------|---------------------------------------------------------|
| `operator.accessKey`                      | AWS Access Key of user that has permission    | ``                                                      |
| `operator.secrtAccessKey=`                | AWS Secret Key of user that has permission    | ``                                                      |
| `operator.bucketName`                     | S3 Bucket Name where folders are created      | ``                                                      |
| `operator.image`                          | The Docker Image Repo for Operator            | ``                                                      |


