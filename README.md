# Lab Logging Software

## QE Logging Software

### Collection

  - Identify all LC-MS instrument logs
  - Collect all LC-MS instrument logs
    - A log refers to a specific log message
    - A log file may contain many logs for some range of time
  - Add useful metadata to logs
    - Save specific log file name and type associated wiht log
    - For instance, a group of logs may relate to a specific experiment, but each log may not include this metadata. Where possible, add such metadata.

### Reporting

  - Create a general or homepage "dashboard" to display network and LC-MS system status
  - Create dashboard for each LC-MS insturment
  - Create dashboard for each network resource
    - i.e., Hazel (FreeNAS), Windows VM workstations, galaxy status
    - [example](https://stats.galaxyproject.eu/d/000000004/galaxy?orgId=1&refresh=5m)
  - Tailor dashboard for each resource
    - e.g., If the logs tell us that the instrument is on sample injection 14 of 80 for an experiment named "Sunflower Oil", we should convey as much of this information possible as clearly as possible--perhaps with a percentage bar.
  - Email relevant admins and/or LC-MS users of urgent and relevant logs

### Documentation

  - General report user documentation
  - Documentation for users to customize report dashboards
  - In-line code documentation
  - Admin documentation for collection
    - Admins should be able to recreate system with this documnetation.
  - Admin documentation for reporting
  - Cohen-Hegeman Network specific documentation
    - How these systems are implemented in our lab.
    - Should include network topology.

## Future bucketlist

- Ansibilize deployment of server
- Create solvent level sensor
- Sample incoming data for anomalies
