# Open Network Source-of-Truth Platform

ONSP(Open Network Source-of-Truth) is a scalable and high available network source-of-truth solution.

## Requirements
- Easy to scale when read/write request rate increase
- Easy to upgrade
- Easy to add new features tested from dev env
- Support dev and prod envs
- Evaluate the read request rate and write request rate

## System Design
### High level design
![alt text](docs/images/high_level.png)
### Components design


## Monitoring
For infras, we should monitoring at least CPU, Memory and Storage. Personally, I'd like to use node_exporter to collect metric from underlying infras.
For services running on the infras, or dockerization env like docker or K8S, we need monitoring the following metrics.
- Requests rate - read/write
- Response time
- Database read rate
- Database write rate
- Error rate

Besides this, we should also collect the logging from both underlying infras and overlaying serices.

## System upgrading

