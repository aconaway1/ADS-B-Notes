# Receivers

## DAH-ADSB01
### Hardware
Raspberry Pi 4GB
### Software
FR24 Image
## DAH-ADSB02
### Hardware
Raspberry Pi 3, 1GB
### Software
ADSBX Image

# Feeds
## FlightRadar24
https://www.flightradar24.com/share-statistics
### Notes
* To upgrade or replace a feeder, you'll need the sharing key, which is found [here](https://www.flightradar24.com/account/data-sharing).
## FlightAware
https://flightaware.com/adsb/stats/user/jaconaway1
### Notes
* FA installs an APT repo to install the feeder.

~~## ADSB Exchange
https://www.adsbexchange.com/myip/~~
## Planefinder
https://planefinder.net/account/receivers
### Notes
* Sharecode can be found in /etc/pfclient-config.json
## Opensky Network
https://opensky-network.org/my-opensky

# Notes
The provider of the image (FR24, ADSBX, etc.) includes a dump1090 utility of some kind. This utility uses the SDR receiver to decode the ADS-B messages and also provides several service ports for other feeds to see what that dump1090 found.

https://github.com/antirez/dump1090

Other feeds include a .DEB package that will read ports 3000[123] to get that data and send it back to their service. These .DEBs are pretty smart and will figure out what's going on without too much effort on your part.
