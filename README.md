# Fluval Bluetooth Hub

By default, it does not build with any light config. In your ESPHome yaml config file, add the following to add either, or both, the `Marine` or `Planted` configuration.

```
substitutions:
  # Change to match your device
  mac_address_marine: '44:A6:E5:68:DA:E9' 
  mac_address_planted: '44:A6:E5:73:23:E3'

packages:
  TheRealFalseReality.fluval_marine:
    url: https://github.com/TheRealFalseReality/fluval-bluetooth-hub
    ref: main
    file: common/fluval_bluetooth_marine.yaml
    refresh: 1h
  TheRealFalseReality.fluval_planted:
    url: https://github.com/TheRealFalseReality/fluval-bluetooth-hub
    ref: main
    file: common/fluval_bluetooth_planted.yaml
    refresh: 1h
```

[ESPHome Documentation](https://deploy-preview-2653--esphome.netlify.app/components/fluval_ble_led.html)
