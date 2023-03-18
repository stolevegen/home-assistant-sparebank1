# Sparebank1 Sensor Platform for Home Assistant

This sensor platform uses the open API of the norwegian bank Sparebank1. 

Every account the customer has in the bank is created as sensor, and updated every 30 minutes.

## Installation

Clone this repository to the `custom_components/sensor/` directory in your Home Assistant config directory.

`git clone git@github.com:trondsundt/home-assistant-sparebank1.git Sparebank1`

Restart your Home Assistant instance to load the component.

## Configuration

1. 
2. Create an app in the developer portal. Store your Client ID somewhere and create a new password (secret).
3. Configure the sensor in Home Assistant.

```yaml
sensor:
    - platform: sparebank1
      customer_id: 01010012345
      client_id: yourClientId
      secret: yourSecret
```

That's it! You can now use your brand new Sparebank1 sensor.

