---
layout: page
title: "UPC ConnectBox"
description: "Instructions on how to integrate UPC ConnectBox into Home Assistant."
date: 2016-12-30 00:00
sidebar: true
comments: false
sharing: true
footer: true
logo: upc.png
ha_category:
  - Presence Detection
ha_release: 0.36
redirect_from:
 - /components/device_tracker.upc_connect/
---


The `upc_connect` platform offers presence detection by looking at connected devices to a [Connect Box](https://www.upc.ch/en/internet/learn-about-internet/) from [Liberty Global](https://www.libertyglobal.com) (also known as UPC Cablecom in Switzerland) which is an Internet provider in Switzerland, Austria and the Netherlands (under Ziggo).

To use a Connect Box in your installation, add the following to your `configuration.yaml` file:

```yaml
# Example configuration.yaml entry
device_tracker:
  - platform: upc_connect
```

{% configuration %}
host:
  description: The IP address of your router.
  required: false
  default: 192.168.0.1
  type: string
{% endconfiguration %}

See the [device tracker component page](/components/device_tracker/) for instructions how to configure the people to be tracked.

Also known to be working with the following devices:
 - Irish Virgin Media Super Hub 3.0
 - Unitymedia Connect Box (DE)
 - Ziggo Connectbox (NL)
 
