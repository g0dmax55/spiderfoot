<a href="https://www.spiderfoot.net/r.php?u=aHR0cHM6Ly93d3cuc3BpZGVyZm9vdC5uZXQv&s=os_gh"><img src="https://www.spiderfoot.net/wp-content/themes/spiderfoot/img/spiderfoot-wide.png"></a>


[![License](https://img.shields.io/badge/license-GPLv2-blue.svg)](https://raw.githubusercontent.com/smicallef/spiderfoot/master/LICENSE)
[![Python Version](https://img.shields.io/badge/python-3.6+-green)](https://www.python.org)
[![Stable Release](https://img.shields.io/badge/version-3.2-blue.svg)](https://github.com/smicallef/spiderfoot/releases/tag/v3.2)
[![CI Status](https://img.shields.io/travis/smicallef/spiderfoot)](https://travis-ci.com/github/smicallef/spiderfoot)
[![Last Commit](https://img.shields.io/github/last-commit/smicallef/spiderfoot)](https://github.com/smicallef/spiderfoot/commits/master)
[![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/github/smicallef/spiderfoot)](https://libraries.io/github/smicallef/spiderfoot)
[![Codecov](https://codecov.io/github/smicallef/spiderfoot/coverage.svg)](https://codecov.io/github/smicallef/spiderfoot)
[![Twitter Follow](https://img.shields.io/twitter/follow/spiderfoot?label=follow&style=social)](https://twitter.com/spiderfoot)

**SpiderFoot** is an open source intelligence (OSINT) automation tool. It integrates with just about every data source available and utilises a range of methods for data analysis, making that data easy to navigate. 

SpiderFoot has an embedded web-server for providing a clean and intuitive web-based interface but can also be used completely via the command-line.  It's written in **Python 3** and **GPL-licensed**.

<img src="https://www.spiderfoot.net/wp-content/uploads/2020/08/SpiderFoot-3.1-browse.png">

### FEATURES

- Web based UI or CLI
- Over 190 modules (see below)
- Python 3
- CSV/JSON/GEXF export
- API key export/import
- SQLite back-end for custom querying
- Highly configurable
- Fully documented
- Visualisations
- TOR integration for dark web searching
- Dockerfile for Docker-based deployments
- Can call other tools like DNSTwist, Whatweb, Nmap and CMSeeK
- Actively developed since 2012!

### USES

SpiderFoot can be used offensively (e.g. in a red team exercise or penetration test) for reconnaissance of your target or defensively to gather information about what you or your organisation might have exposed over the Internet.

You can target the following entities in a SpiderFoot scan:

 - IP address
 - Domain/sub-domain name
 - Hostname
 - Network subnet (CIDR)
 - ASN
 - E-mail address
 - Phone number
 - Username
 - Person's name
 
SpiderFoot's 190+ modules feed each other in a publisher/subscriber model to ensure maximum data extraction to do things like:

- [Host/sub-domain/TLD enumeration/extraction](https://asciinema.org/a/295912)
- [Email address, phone number and human name extraction](https://asciinema.org/a/295947)
- [Bitcoin and Ethereum address extraction](https://asciinema.org/a/295957)
- [Check for susceptibility to sub-domain hijacking](https://asciinema.org/a/344377)
- DNS zone transfers
- [Threat intelligence and Blacklist queries](https://asciinema.org/a/295949)
- API integration with [SHODAN](https://asciinema.org/a/127601), [HaveIBeenPwned](https://asciinema.org/a/128731), [GreyNoise](https://asciinema.org/a/295943), AlienVault, SecurityTrails, etc.
- [Social media account enumeration](https://asciinema.org/a/295923)
- [S3/Azure/Digitalocean bucket enumeration/scraping](https://asciinema.org/a/295941)
- IP geo-location
- Web scraping, web content analysis
- [Image, document and binary file meta data analysis](https://asciinema.org/a/296274)
- Dark web searches
- [Port scanning and banner grabbing](https://asciinema.org/a/295939)
- [Data breach searches](https://asciinema.org/a/296145)
- So much more...

### INSTALLING & RUNNING

To install and run SpiderFoot, you need at least Python 3.6 and a number of Python libraries which you can install with `pip`. We recommend you install a packaged release since master will often have bleeding edge features and modules that aren't fully tested.

 #### Development build (cloning git master branch): 
```
$ git clone https://github.com/keralahacker/spiderfoot.git
$ cd spiderfoot
$ pip3 install -r requirements.txt
~/spiderfoot$ python3 ./sf.py -l 127.0.0.1:5001
```

#### one line command 👇🏻  for Termux 

```
git clone https://github.com/smicallef/spiderfoot.git && cd spiderfoot && pip3 install -r requirements.txt && python3 -m pip install --upgrade pip && python3 ./sf.py -l 127.0.0.1:5001
```


$ wget https://github.com/keralahacker/spiderfoot/archive/v3.2.tar.gz
$ tar zxvf v3.2.tar.gz
$ cd spiderfoot
~/spiderfoot$ pip3 install -r requirements.txt
~/spiderfoot$ python3 ./sf.py -l 127.0.0.1:5001
```

#### Development build (cloning git master branch):

```
$ git clone https://github.com/keralahacker/spiderfoot.git
$ cd spiderfoot
$ pip3 install -r requirements.txt
~/spiderfoot$ python3 ./sf.py -l 127.0.0.1:5001
```

