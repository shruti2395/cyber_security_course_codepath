# Week 10 & 11 - Project: Honeypot

## Setup

- Installed MHN Admin on Droplet from DigitalOcean cloud provider on Ubuntu 16.04
- Installed 3 Honeypot servers and let them run overnight

## Honeypots tried

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


## Issues encountered
- MHN Admin did not work with Ubuntu 18.04 instance. I tried running it with Ubuntu 16.04 version
- Dionaea over HTTP setup did not work from the Deploy script. Found another steps at https://www.attacusatlas.com/how-to-set-up-dionaea-honeypot-to-evade-nmap-detection/ 
