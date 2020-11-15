# Netgear

## To turn on/off 2.4GHz wireless radio

Go to Advanced > Advanced Setup > Wireless Settings > 2.4GHz b/g/n and click Enable Wireless Router Radio

## Change time

Go to Advanced > Administration > NTP Settings. Choose your time zone and check "Automatically adjust for daylight savings time".

## Block service for a specific device

1. Go to Advanced > Setup > LAN Setup > Address Reservation. Click Add, pick the MAC address for your device and enter a relevant name.
1. Go to Advanced > Security > Block Services. Select "Per Schedule" and click Add.
1. For Protocol, select "TCP/UDP".
1. For Starting Port and Ending Port, enter 1 and 65535.
1. Under "Filter Services For:" select "Only this IP address".
1. Go to Advanced > Security > Schedule. Uncheck "All day". Enter start and end blocking times.

Source: https://community.netgear.com/t5/Nighthawk-WiFi-Routers/Blocking-device-based-on-time-schedule/td-p/1200925#
