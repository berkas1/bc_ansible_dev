## Grafana for Visualisation (Ansible)

**This is experimental repository and errors may occur. Use for testing purposes only for now.**

To try-out Grafana easily (see [Grafana for Visualisation](https://www.bigclown.com/doc/integrations/grafana-for-visualization/) in documentation) you can use Vagrant to deploy virtual machine with prepared environment.

This repository contains predefined `Vagrantfile` and Ansible playbook which takes care of the Grafana & InfluxDB installation as described in the linked article. 

### How to Use
Use is pretty simple. On your host machine `ansible` and `vagrant` have to be installed. Then:

1. Clone this repository
2. run `vagrant up`
3. Now wait until the installation is completed. 


### Networking
You virtual machine is available from your entire network, not just from the host computer.

#### Port forwarding
Some ports are forwarded to host machine:

| Guest (virtual) machine | Host machine |
|-------------------------|-------------:|
| 8086                    | 20000        |
| 8088                    | 20001        |
| 3000                    | 20002        |