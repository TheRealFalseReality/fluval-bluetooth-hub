# Fluval Bluetooth Hub

By default, it does not build with any light config. In your ESPHome yaml config file, add the following to add either, or both, the `Marine` or `Planted` configuration.

```
substitutions:
  # Change to match your device
  mac_address_marine: '44:A6:E5:68:DA:E9' 
  mac_address_planted: '44:A6:E5:73:23:E3'
  # dhtPin: '25'

packages:
  # Add Either or Both
  TheRealFalseReality.fluval_hub_marine: github://TheRealFalseReality/fluval-bluetooth-hub/common/fluval_bluetooth_marine.yaml@main
  TheRealFalseReality.fluval_hub_planted: github://TheRealFalseReality/fluval-bluetooth-hub/common/fluval_bluetooth_planted.yaml@main

  # Debug (Optional, Uncomment to Add)
  # TheRealFalseReality.debug: github://TheRealFalseReality/fluval-bluetooth-hub/common/debug.yaml@main

  # DHT (Optional, why not?)
  # TheRealFalseReality.dht: github://TheRealFalseReality/fluval-bluetooth-hub/common/dht.yaml@main
```

[ESPHome Documentation](https://deploy-preview-2653--esphome.netlify.app/components/fluval_ble_led.html)
