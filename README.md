
Ubuntu 32-bit Images for Docker
===============================

The [Ubuntu 32-bit images for Docker](https://github.com/f69m/docker-ubuntu32) are built the same way as the official Docker Ubuntu 64-bit images. They are based on the Ubuntu cloud images released by Canonical.

For available tags please see the [list of tags at Docker Hub](https://hub.docker.com/r/f69m/ubuntu32/tags/).

## Usage

The images are mainly useful to derive other images from, but can be used standalone like:

    $ docker pull f69m/ubuntu32:lts
    $ docker run --rm -it f69m/ubuntu32:lts bash

## Branches

The `master` branch contains only scripts and config files and has a proper Git history. The `dist` branch contains the big binary blobs for building the images and will always be a single commit on top of the `master` branch.

## Contribute

You are welcome to discuss these images, report any issues or contribute changes here on Github, but please stick to topics specific to the 32-bit Docker images. More general contributions should be directed upstream.

Pull requests should only be done for scripts and config files against the `master` branch. Please do not create pull requests agains the `dist` branch.

## Why 32-bit?

So why make the effort to create 32-bit images? All the nice stuff out there is built for a 64-bit architecture.

Two reasons: for one I sometimes work on an old 32-bit laptop, so running anything with Docker requires 32-bit images.

And then using 32-bit images saves a lot of memory, with negligible impact on the performance. Unless your application is one of the few that can really benefit from 64-bit instructions. So 32-bit images allow running more containers on a cheap VPS. This does save real
money!

