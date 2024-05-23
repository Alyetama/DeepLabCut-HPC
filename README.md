![Docker](https://github.com/bchaselab/DeepLabCut-Slurm/workflows/Docker/badge.svg) ![Docker Image CI](https://github.com/bchaselab/DeepLabCut-Slurm/workflows/Docker%20Image%20CI/badge.svg) ![Docker Pulls](https://img.shields.io/docker/pulls/fcatus/deeplabcut) ![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/fcatus/deeplabcut)

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

## Build From a Singularity [Definition File](https://sylabs.io/guides/3.5/user-guide/definition_files.html)

```shell
# Download the definition file
$ wget https://gist.githubusercontent.com/Alyetama/c819bb2d07e58b47208c69ce76c22feb/raw/c07b264adc5424d6bd939a77bb34a95a6f80dca1/dlc.def

# Customize the definition file (optional)
$ vim dlc.def

# Build remotely from the definition file
$ singularity build --remote deeplabcut.sif dlc.def
```

For more information about using `singularity build`, see [Singularity Build](https://sylabs.io/guides/3.1/user-guide/cli/singularity_build.html).
