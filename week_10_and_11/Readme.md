# Week 10 & 11 - Project: Honeypot

## Setup

- Installed MHN Admin on Droplet from DigitalOcean cloud provider on Ubuntu 16.04
- Installed 3 Honeypot servers and let them run overnight

![droplet instances](https://github.com/shruti2395/cyber_security_course/raw/master/week_10_and_11/digital_ocean_instances.png "Digital Ocean instances")

![attack report](https://github.com/shruti2395/cyber_security_course/raw/master/week_10_and_11/attacks_report.png "Attack Report")

![payload report](https://github.com/shruti2395/cyber_security_course/raw/master/week_10_and_11/payloads_report.png "Payload Report")

## Honeypots tried

![sensors page](https://github.com/shruti2395/cyber_security_course/raw/master/week_10_and_11/sensors_page.png "Sensors Page")

### Dionaea
Deployed by following commands in the blog post mentioned below.
Received ~3000 attacks in 10 hours.

### Ubuntu Shockpot
Deployed from commands in the MHN Deploy page.
Did not receive any attacks in 10 hours.

### Ubuntu Wordpot
Deployed from commands in the MHN Deploy page.
Did not recieve any attacks in 10 hours.

## Data exported

![top attacks page](https://github.com/shruti2395/cyber_security_course/raw/master/week_10_and_11/top_attacks.png "Top Attacks")

Session export data is at https://github.com/shruti2395/cyber_security_course/raw/master/week_10_and_11/session.json

## Issues encountered
- MHN Admin did not work with Ubuntu 18.04 instance. I tried running it with Ubuntu 16.04 version
- Dionaea over HTTP setup did not work from the Deploy script. Found another steps at https://www.attacusatlas.com/how-to-set-up-dionaea-honeypot-to-evade-nmap-detection/ 

## Settings page

![settings page](https://github.com/shruti2395/cyber_security_course/raw/master/week_10_and_11/settings_page.png "Settings Page")
