# hof
Hacker one fetcher, fetch hacker one projects and get subdomains and heders for all scope domains.

## Installation

`cargo install hof`

## Dependencies

findomain: https://github.com/Findomain/Findomain

## Configure vpn switching feature:

In the config file you can specify if
you want the program to reconnect your vpn server
every couple requests, this can shorten the time that it takes
to fetch a large chunk of domains from the same server, this is the default config file:
```
{
  "use_vpn": false,
  "vpn_cmd": "",
  "vpn_loop": 25,
  "vpn_reconnect_delay": 10
}

```
If you want to use this feature change the "use_vpn" key to true.
in the "vpn_cmd" key specify a command to restart the vpn
you are using, for example for openvpn you would use: "service openvpn restart".
in the "vpn_loop" specify in how many requests you want to restart the vpn
for example the default 25 means every 25 requests the program will restart the vpn.
in the "vpn_reconnect_delay" specify how many seconds you want the progream to 
wait after reconnecting the vpn.

## Command arguments:

```
USAGE:
    hof [OPTIONS] --query <QUERY> --path <PATH>

OPTIONS:
    -h, --help                 Print help information
    -p, --path <PATH>          A path you want your project to be saved at
    -q, --query <QUERY>        A query for hackerone
    -t, --timeout <TIMEOUT>    Set timeout for each request in seconds [default: 8]
    -V, --version              Print version information
```
