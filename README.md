# Shepherd
A InfluxDB database and Grafana frontend for lab log storage and visualization.
 
## Motivation
The goal is to have real-time and historical monitoring of the lab's instrument logbooks so that machine performance and status can be evaluated.

## Screenshots

## Tech used
[InfluxDB](https://www.influxdata.com/)

[Grafana](https://grafana.com/)

## Installation
1. Install Grafana, InfluxDB, and Collectd
```
apt-get install -y software-properties-common
add-apt-repository "deb https://packages.grafana.com/oss/deb stable main"
wget -q -O - https://packages.grafana.com/gpg.key | apt-key add -
apt-get update
apt upgrade
apt install influxdb grafana collectd
```
2. Place influxdb.conf from this repository in /etc/influxdb 
3. Place types.db from this repository in /etc/share/collectd
4. Place collectd.conf from this repository in /etc/collectd 
## References

