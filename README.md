# Bermuda-Proxies
ESPHome packages for creating BLE Proxies that work well with Bermuda.

These package files are designed to:
- Make creating a proxy easy
- Ensure you get the best performance from the device
- Provide fast and frequent updates to Home Assistant (and therefore to
  Bermuda).

# How to use

For each MCU type, there is a "full" package and a "minimal" package.
The "full" package includes everything you need to flash a bare board
and get up and running with a proxy tuned for Bermuda.

The "minimal" package is ideal if you want to add bluetooth proxy to an
esphome device you have already flashed. You can just add this to your
existing config and it won't stomp all over it :-)

You can view the actual settings used in the [packages](/packages/)
folder, and explanations of the various settings on the [Bermuda
Wiki](https://github.com/agittins/bermuda/wiki/ESPHome-Configurations)

### Classic ESP32 devices (ESP32-ROVER, ESP32-WROOM, Atom Lite ESP32 etc)

To add Bermuda-friendly bluetooth proxy to an existing esphome yaml, add
this section to the yaml and install it:

```yaml
packages:
  Bermuda.esp32: github://agittins/bermuda-proxies/packages/bermuda-proxy-esp32-orig-minimal.yaml

```

### ESP32-S3 (M5Stack CoreS3, AtomS3 Lite etc)

To add Bermuda-friendly bluetooth proxy to an existing esphome yaml, add
this section to the yaml and install it:

```yaml
packages:
  Bermuda.esp32: github://agittins/bermuda-proxies/packages/bermuda-proxy-esp32-s3-minimal.yaml

```

### ESP32-C3 (M5Stack STAMP-C3 etc)

To add Bermuda-friendly bluetooth proxy to an existing esphome yaml, add
this section to the yaml and install it:

```yaml
packages:
  Bermuda.esp32: github://agittins/bermuda-proxies/packages/bermuda-proxy-esp32-c3-minimal.yaml

```
