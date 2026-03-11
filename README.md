# Wardial

This project scans all IP addresses assigned to North Korea and identifies which ones host active web servers.

![Tests](https://github.com/abedoya-norena/Wardial/actions/workflows/python-tests.yml/badge.svg)

## Description

This program performs a simple "war dial" of the DPRK IP address range (175.45.176.0 – 175.45.179.255) and reports which IP addresses are hosting active web servers.

## Example Output

```
$ python3 wardial.py
Scanning: 175.45.176.0
...
Scanning: 175.45.179.255
dprk_ips_with_servers= [
    '175.45.176.68',
    '175.45.176.75',
    '175.45.176.76',
    '175.45.177.1',
    '175.45.177.10',
    '175.45.177.11'
]
```

These are the IP addresses in the DPRK range that responded with an HTTP 200 status code during the scan.