# Install Build Dependencies

```shell
apt update
apt install meson, build-essential
```

# Install Gstreamer Rockchip

```shell
cd gstreamer-rockchip

meson setup build --prefix=/usr

meson compile -C build

meson install -C build
```

# Test Gstreamer Rockchip

```shell
gst-inspect-1.0 --plugin | grep mpp
```
