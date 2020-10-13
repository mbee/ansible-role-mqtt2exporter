# ansible role to install mqtt2exporter

## How to run it

create a playbook and setup on your inventory variables:

| ansible variable              | environment variable | default                  |
| ----------------------------- | -------------------- | ------------------------ |
| mqtt2exporter_mqtt_url        | MQTT_URL             | localhost:1883           |
| mqtt2exporter_mqtt_user       | MQTT_USER            |                          |
| mqtt2exporter_mqtt_password   | MQTT_PASSWORD        |                          |
| mqtt2exporter_prometheus_url  | PROMETHEUS_URL       | 0.0.0.0:2121             |
| mqtt2exporter_prometheus_path | PROMETHEUS_PATH      | /metrics                 |
| mqtt2exporter_device_path     | DEVICE_PATH          | /opt/mqtt2prometheus/etc |

they will be replaced by the corresponding environment variable thanks to the systemctl service.
