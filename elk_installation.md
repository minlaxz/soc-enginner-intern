**ELK** INSTALLATION
===

# L
> ## Installation of **Logstash**
> + check your Java version, `java --version` 
>   + if java exists , _pass_
>   + else , `apt search java`, `sudo apt install {java---}`

> + Import the Elastic PGP Keyedit
>   + Download and install the public signing key: **4609 5ACC 8548 582C 1A26 99A9 D27D 666C D88E 42B4**<br>
`wget -qO - https://artifacts.elastic.co/GPG-KEY-elasticsearch | sudo apt-key add -`

> + Installing from the APT repository
>   + install the *apt-transport-https* package on Debian before proceeding:<br>
`sudo apt-get install apt-transport-https`
>   + Save the repository definition to */etc/apt/sources.list.d/elastic-7.x.list:*<br>
`echo "deb https://artifacts.elastic.co/packages/7.x/apt stable main" | sudo tee -a /etc/apt/sources.list.d/elastic-7.x.list`

> + You can install the **Elasticsearch** Debian package with:
>   + `sudo apt-get update && sudo apt-get install kibna`

> ## Enable automatic creation of system indices.
> + Check **systemd**<br>
`ps -p 1`
> + Kibana **enable**<br>
`sudo /bin/systemctl daemon-reload`<br>
`sudo /bin/systemctl enable kibana.service`
> + ES *start_stop*<br>
`sudo systemctl start kibana.service`<br>
`sudo systemctl stop kibana.service`<br>
`sudo systemctl status kibana.service`



# E
> ## Install **ElasticSearch** (ES) for short.
> + Import the Elastic PGP Keyedit
>   + Download and install the public signing key: **4609 5ACC 8548 582C 1A26 99A9 D27D 666C D88E 42B4**<br>
`wget -qO - https://artifacts.elastic.co/GPG-KEY-elasticsearch | sudo apt-key add -`
> + Installing from the APT repository
>   + install the *apt-transport-https* package on Debian before proceeding:<br>
`sudo apt-get install apt-transport-https`
>   + Save the repository definition to */etc/apt/sources.list.d/elastic-7.x.list:*<br>
`echo "deb https://artifacts.elastic.co/packages/7.x/apt stable main" | sudo tee -a /etc/apt/sources.list.d/elastic-7.x.list`
> + You can install the **Elasticsearch** Debian package with:
>   + `sudo apt-get update && sudo apt-get install elasticsearch`

> ## Enable automatic creation of system indices.
> + Check **systemd**<br>
`ps -p 1`
> + ES **enable**<br>
`sudo /bin/systemctl daemon-reload`<br>
`sudo /bin/systemctl enable elasticsearch.service`
> + ES *start_stop*<br>
`sudo systemctl start elasticsearch.service`<br>
`sudo systemctl stop elasticsearch.service`<br>
`sudo systemctl status elasticsearch.service`

---
# K
> ## Installation of **KIBANA**
> + Import the Elastic PGP Keyedit
>   + Download and install the public signing key: **4609 5ACC 8548 582C 1A26 99A9 D27D 666C D88E 42B4**<br>
`wget -qO - https://artifacts.elastic.co/GPG-KEY-elasticsearch | sudo apt-key add -`
> + Installing from the APT repository
>   + install the *apt-transport-https* package on Debian before proceeding:<br>
`sudo apt-get install apt-transport-https`
>   + Save the repository definition to */etc/apt/sources.list.d/elastic-7.x.list:*<br>
`echo "deb https://artifacts.elastic.co/packages/7.x/apt stable main" | sudo tee -a /etc/apt/sources.list.d/elastic-7.x.list`
> + You can install the **Elasticsearch** Debian package with:
>   + `sudo apt-get update && sudo apt-get install kibna`

> ## Enable automatic creation of system indices.
> + Check **systemd**<br>
`ps -p 1`
> + Kibana **enable**<br>
`sudo /bin/systemctl daemon-reload`<br>
`sudo /bin/systemctl enable kibana.service`
> + ES *start_stop*<br>
`sudo systemctl start kibana.service`<br>
`sudo systemctl stop kibana.service`<br>
`sudo systemctl status kibana.service`

---


---
**sitemap**
+ [logstach install]("https://www.elastic.co/guide/en/logstash/current/installing-logstash.html")
+ [ES install]("https://www.elastic.co/guide/en/elasticsearch/reference/current/deb.html")
+ [kibana install]("https://www.elastic.co/guide/en/kibana/current/install.html")

note:
it is called ELK, but I call it LEK for some reason :D.