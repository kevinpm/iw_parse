iw_parse
========

Parse the output of iw scan to get the name, address, quality, channel, and encryption type of all networks broadcasting within your Wireless NIC's reach.


```

Usage
-----

```bash
iw <INTERFACE_NAME> scan | ./iw_parse
```

Replace `<INTERFACE_NAME>` with the system name for your wireless NIC. It is usually something like `wlan0`. The command `iwconfig` will list all of your network interfaces.

Example:

```bash
iw wlan0 scan | ./iw_parse
```

The result should look something like:

```
SSID             BSSID                Channel   
wireless1        20:AA:4B:34:2C:F5    11        
wireless2        00:26:F2:1E:FC:03    1         
wireless3        00:1D:D3:6A:3C:60    6         
wireless4        20:10:7A:E5:02:98    1         
wireless5        CC:A4:62:B7:D2:B0    8         
wireless6        30:46:9A:53:3C:76    11        
wireless7        A0:21:B7:5F:84:B0    11        
wireless8        04:A1:51:18:E8:E0    6         
```


Acknowledgements
----------------

* The vast majority of iw_parse was written by Hugo Chargois.
* It was then forked to run with iw command by Kevin Perez.

License
-------

iw_parse is free--as in BSD. Hack your heart out, hackers.
