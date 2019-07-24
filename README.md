# Shepherd
A InfluxDB database and Grafana frontend for lab log storage and visualization.
 
## Motivation
The goal is to have real-time and historical monitoring of the lab's instrument logbooks so that machine performance and status can be evaluated.

## Screenshots
#### Grafana home page
![Grafana home page](https://github.com/HegemanLab/shepherd/raw/master/Grafana%20Home%20Page.png)
#### A simple text filled grafana dashboard
![A simple text filled grafana dashboard](https://github.com/HegemanLab/shepherd/raw/master/Grafana%20Bruker%20Dashboard.png)
#### A temperature and pressure mapping dashboard
![A temperature and pressure mapping dashboard](https://github.com/HegemanLab/shepherd/raw/master/Grafana%20QE%20Temperature.png)

## Tech used
[InfluxDB](https://www.influxdata.com/)

[Grafana](https://grafana.com/)

## Installation
1. Install Grafana, InfluxDB, and Collectd
```
# install dependencies
apt-get install -y software-properties-common

# add Grafana repo
add-apt-repository "deb https://packages.grafana.com/oss/deb stable main"

# add Grafana repo key and add it to apt-key
wget -q -O - https://packages.grafana.com/gpg.key | apt-key add -

# update apt's cache
apt-get update

# install
apt install influxdb grafana collectd
```
2. Place influxdb.conf from this repository in `/etc/influxdb`
3. Place types.db from this repository in `/etc/share/collectd`
4. Place collectd.conf from this repository in `/etc/collectd`
5. Run the following commands to start influxdb, collectd, and grafana as a systemctl service
```
 systemctl start influxdb
 systemctl start collectd
 systemctl start grafana-server
```
## References

