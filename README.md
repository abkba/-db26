# DefCon 26
Stuff done at DefCon26

- Vagrant setup:
  - 1 nat-node
    - node has netdata installed
    - forwarding port 19999 to localhost
  - 2 clients routing out of nat node
  - TODO
    - setup graphite node properly with statsd
    - grafana with statsd as backend (Ansible?)
  
- Python script to aggregate data from /proc/net/nf_conntrac file
  - tested using `pynetfilter_conntrack` library to no avail
  - TODO
    - going to hack together a shitty script that aggregates data from above file and sends it to graphite/statsd endpoint.
