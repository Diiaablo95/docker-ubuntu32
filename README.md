
# Ubuntu 32-bit Container for Docker

The [Ubuntu 32-bit containers for Docker](https://github.com/f69m/docker-ubuntu32)
are built the same way as the official Docker Ubuntu 64-bit containers
based on the Ubuntu cloud images released by Canonical.

For available tags please see .

## Usage

The images are mainly useful to derive other images from, but can be
used standalone like:

```
$ docker pull f69m/ubuntu32:lts
$ docker run --rm -it f69m/ubuntu32:lts bash
```

## Branches

The `master` branch contains only scripts and config files and has a
proper Git history. The `dist` branch contains the big binary blobs
for building the images and will always be a single commit on top of
the `master` branch.

## Contribute

You are welcome to discuss these images, report any issues or
contribute changes here on Github, but please stick to topics specific
to the 32-bit Docker images. More contributions should be directed
upstream.

Pull requests should only be done for scripts and config files against
the master branch. Please do not create pull requests agains the dist
branch.

