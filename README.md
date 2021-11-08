# NOC-Compose-InfluxDB-Grafana
This is a multi-container compose confiugration for InfluxDB 2.0 (Latest) and Grafana Enterprise:Alpine (Latest)

This is useful for quicklly validating telegraf agent configurations that require influxDB and the validation of community grafan daahboards, especially those requiring Telegraf as a collector and InfluxDB as a data source.

## Quick Start

To start the app:

1. Install [docker-compose](https://docs.docker.com/compose/install/) on the docker host.
2. Clone this repo on the docker host.
3. Create a .env file in the top level folder/root of the repository.
4. Run the following command from the root of the cloned repo:

`docker-compose up -d`

## .env file for variable references
The .env file specifies a pre-created Grafana and InfluxDB user for persistent referencing. The referenced variables are:

- INFLUXDB_USERNAME
- INFLUXDB_PASSWORD
- GRAFANA_USERNAME
- GRAFANA_PASSWORD

These must reference or initalised in .env file like so
- `INFLUXDB_USERNAME=xxxxx`
- `INFLUXDB_PASSWORD=xxxxx`
- `GRAFANA_USERNAME=xxxxx`
- `GRAFANA_PASSWORD=xxxxxx`
