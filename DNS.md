# DNS Troubleshooting

Some basic things to do when you have DNS problems.

## Get IP address for a domain

`dig feihonghsu.com +short`

## Check nameservers for a domain

`dig @8.8.8.8 +short NS feihonghsu.com`

## Query a specific nameserver

`dig @ns1.webfaction.com feihonghsu.com +short`

## Sources

- [Use dig to query nameservers](https://support.rackspace.com/how-to/using-dig-to-query-nameservers/)
- [DiG HOWTO](https://www.madboa.com/geek/dig/)
