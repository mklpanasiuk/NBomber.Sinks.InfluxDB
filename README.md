[![Build status](https://ci.appveyor.com/api/projects/status/ptahoo3renvkn7vu?svg=true)](https://ci.appveyor.com/project/PragmaticFlowOrg/nbomber-sinks-influxdb)
[![NuGet](https://img.shields.io/nuget/v/nbomber.sinks.influxdb.svg)](https://www.nuget.org/packages/nbomber.sinks.influxdb/)
[![Gitter](https://badges.gitter.im/nbomber/community.svg)](https://gitter.im/nbomber/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

A NBomber sink that writes statistics to InfluxDB.

### How to install
To install NBomber.Sinks.InfluxDB via NuGet, run this command in NuGet package manager console:
```code
PM> Install-Package NBomber.Sinks.InfluxDB
```

### Documentation
Documentation is located [here](https://nbomber.com/docs/).

### Contributing
Would you like to help make NBomber even better? We keep a list of issues that are approachable for newcomers under the [good-first-issue](https://github.com/PragmaticFlow/NBomber.Sinks.InfluxDB/issues?q=is%3Aopen+is%3Aissue+label%3A%22good+first+issue%22) label.

### Examples
An example is located [here](https://github.com/PragmaticFlow/NBomber.Sinks.InfluxDB/tree/master/examples).

### docker-compose
docker-compose is located in `docker-compose` direactory and contains the following services:
* [InfluxDB 1.x](https://github.com/influxdata/influxdb) - an open-source time series platform.
Please note, InfluxDB 2.x is not supported so far but docker-compose for this version is located under directory `docker-compose2` (with no grafana dashboards).
* [Grafana](https://github.com/grafana/grafana) - an open-source platform for monitoring and observability.
`Grafana` contains provisioning for `InfluxDB` datasource and `NBomber` dashboard.
Credentials can be found in `.env` file.

### Quick Start
To run the example:
1. Install [Docker Compose](https://docs.docker.com/compose/install/).
2. Clone this repository.
3. Execute the following command from `docker-compose` directory:
```code
docker-compose up -d
```
4. Run the example.
5. Open `Grafana` in a browser (http://localhost:3000/) and observe `NBomber` dashboard.

To stop services:
1. Execute the following command from `docker-compose` directory:
```code
docker-compose down
```
