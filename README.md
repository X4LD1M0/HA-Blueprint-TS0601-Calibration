# Temperature Calibration Zigbee TS0601

This blueprint uses an external temperature sensor to calibrate a Zigbee TS0601 which is connected to Zigbee2MQTT. It is slightly different from the ones previous found in the Blueprint section of the Home Assistant forum, since those expect the "local_temperature_calibration" attribute to be part of the TS0601 entity itself.

When in Zigbee2MQTT the "Home Assistant legacy entity attributes" is disabled, when disabled Zigbee2MQTT will _NOT_ add state attributes to each entity, therefore there is no 'local_temperature_calibration' attribute in the TS0601 entity.

Using this Blueprint the following entities have to be provided;

- TS0601 radiator valve with thermostat
- External temperature sensor
- local_temperature_calibration entity (of the TS0601 element)
