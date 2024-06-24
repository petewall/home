# Telemetry

Gathers telemetry data from the Synology and sends it to Grafana Cloud.

## Deployment

1. Install the [Container Manager](https://www.synology.com/dsm/packages/ContainerManager) package.
1. Generate the secrets with `make config.env`.
1. In File Station, Upload `config.alloy` and `config.env` to `/volume1/docker/container-configs/telemetry`.
1. In Container Manager, create a new Project, named `telemetry` and use the `docker-compose.yaml` file for the definition.
    * NOTE: You cannot build this config with the wizard, you need the `docker-compose.yaml` file. That's because it needs volume mounts that aren't available in the wizard.
