# dns
[![CircleCI status](https://img.shields.io/circleci/project/github/uubk/dns/master.svg?style=shield)](https://circleci.com/gh/uubk/dns/tree/master)
![License](https://img.shields.io/github/license/uubk/dns.svg?style=popout)

Configures DNS entries for the target machine. This assumes that DNS entries can be edited using `nsupdate` and a host keytab.

## Configuration
| Name | Default value | Description |
| ---- | ------------- | ----------- |
| `dns_store_ssh_fingerprint` | `True` | Whether to deploy `SSHFP` records for the host in DNS |
| `dns_do_dynamic_dns` | `False` | Whether to update A and AAAA records of the host regularly |
| `dns_dynamic_dns_v4` | `""` | When using dynamic DNS, this URL should return the IPv4 of the host |
| `dns_dynamic_dns_v6` | `""` | When using dynamic DNS, this URL should return the IPv6 of the host |
| `dns_servers` | `[]` | Array of servers that can take DNS update requests. One will be choosen at random at deployment time |

## License
GPLv3
