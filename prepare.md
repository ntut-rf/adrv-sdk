# Prepare

## Install system packages

```shell-session
$ sudo apt install git gcc make cmake ccache rsync \
    libfmt-dev libspdlog-dev libyaml-cpp-dev \
    gnuradio-dev libuhd-dev uhd-host \
    libprotobuf-dev libprotoc-dev protobuf-compiler nodejs npm nlohmann-json3-dev \
    libgtk-3-dev libwebkit2gtk-4.0-dev
```

<!-- slide:break -->

# 

## Setup UHD (for USRP)

Download USRP images:
```shell-session
$ sudo uhd_images_downloader
```

Setup USRP permissions:
```shell-session
$ sudo cp /usr/lib/uhd/utils/uhd-usrp.rules /etc/udev/rules.d/10-uhd-usrp.rules
```