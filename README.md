![Docker](https://github.com/bchaselab/DLC-Docker/workflows/Docker/badge.svg) ![Docker Image CI](https://github.com/bchaselab/DLC-Docker/workflows/Docker%20Image%20CI/badge.svg)

## From [Dockerhub](https://hub.docker.com/repository/docker/fcatus/deeplabcut)
```shell
$ docker pull fcatus/deeplabcut:latest
```

## To Use With Singularity
```shell
$ singularity pull docker://fcatus/deeplabcut:latest
```

or build it from a singularity file

```shell
$ vim singularity
```

```yaml
Bootstrap: docker
From: fcatus/deeplabcut:latest
```

```shell
$ singularity build --remote deeplabcut.sif singularity
```

For more information about using `singularity build`, see [Singularity Build](https://sylabs.io/guides/3.1/user-guide/cli/singularity_build.html).
