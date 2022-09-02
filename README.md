# SISO2

## Setup

### Install prerequisites

```
$ sudo apt install git gcc make cmake ccache libfmt-dev libspdlog-dev libyaml-cpp-dev gnuradio-dev libuhd-dev uhd-host libprotobuf-dev libprotoc-dev protobuf-compiler nodejs npm libgtk-3-dev libwebkit2gtk-4.0-dev rsync
$ sudo uhd_images_downloader
$ sudo cp /usr/lib/uhd/utils/uhd-usrp.rules /etc/udev/rules.d/10-uhd-usrp.rules
```

### Clone and update submodules

```
$ git clone git@github.com:ntut-rf/SISO2.git
$ cd SISO2/
$ git submodule init
$ git submodule update
```

### Build

```
$ make -j
```

## Usage

### Host (USRP)

```
$ ./bin/siso2
```

### ADRV9364

Navigate to http://adrv.local

## Configuration

### Host (USRP)

`./config.yaml`

### ADRV9364

`/etc/siso2.yaml`

## References

* [A936x IIO reference](https://wiki.analog.com/resources/tools-software/linux-drivers/iio-transceiver/ad9361)
