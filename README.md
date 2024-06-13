# RPi4 setup for Brunnshög

## Flash drive

### Using cli tools

Download image from http://cdimage.ubuntu.com/releases/20.04/release/

``` sh
curl http://cdimage.ubuntu.com/releases/20.04/release/ubuntu-20.04.5-preinstalled-server-arm64+raspi.img.xz -o raspi.img.xz
```

Copy to drive

``` sh
xzcat raspi.img.xz | dd of=/dev/sdX status=progress
```

### Using Raspberry Pi Imager

Install [Raspberry Pi Imager](https://www.raspberrypi.com/software/).

Select model and OS (Ubuntu 20.04 arm64)

## Setup cloud-ini

Move files in the cloud-init directory to the root of the flashed drive.
