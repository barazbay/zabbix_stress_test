# zabbix_stress_test
## Prepare zabbix server
Ensure cache configurations are good enough
## Prepare zabbix web server
Ensure upload settings are good enough
## Prepare hosts
You will basically need a template with the item proc.num[]

I used "Template OS Linux" from stock zabbix server installation for it.
All generated items depend from proc.num[]
## Server version
server version must be 4.2.0+
tested on 
zabbix server 4.2.6 without proxy
## Usage
Just install "Template OS Linux" and one ore more templates on linux host. This stress test is valid only for server and database. Zabbix agent will not be loaded since all items are generated.

## Source
I used an idea from this repo 
https://github.com/monitoringartist/zabbix-server-stress-test