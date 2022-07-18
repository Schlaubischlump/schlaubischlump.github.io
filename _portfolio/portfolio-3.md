---
title: "shairport-metadatareader-python"
excerpt: "A shairport-metadata-reader package written in Python, which supports reading the metadata from the pipe file, the UDP-server and the MQTT server if configured."
collection: portfolio
---

This python (>= 2.7 or >= 3.4) library includes a package shairportmetadatareader which parses the airplay metadata from the shairport-sync pipe, the specified shairport-sync udp server or the shairport-sync mqtt server. In addition, it includes a remote sub-package to remotely control the Airplay client.

## Example to read metadata
```Python
from time import sleep
from shairportmetadatareader import AirplayUDPListener #, AirplayPipeListener

def on_track_info(lis, info):
    """
    Print the current track information.
    :param lis: listener instance
    :param info: track information
    """
    print(info)

listener = AirplayUDPListener() # You can use AirplayPipeListener or AirplayMQTTListener
listener.bind(track_info=on_track_info) # receive callbacks for metadata changes
listener.start_listening() # read the data asynchronously from the udp server
sleep(60) # receive data for 60 seconds
listener.stop_listening()
```

For more information check out [the github page](https://github.com/Schlaubischlump/shairport-metadatareader-python).
