# check_mx_all_flavours

## Usage

```sh
check_mx_all_flavours <domain>"
```

It may be helpful to pipe the output though `column -t`

## Description

check all mx hosts of the given domain for

* reachability over ipv4 and ip6
* support for starttls
* support for TLS 1.2 and TLS 1.3
* support for RSA and ECDSA certificates
* whether the certificates are trusted
* whether DANE data are available and valid

The program is expected to be run on a system capable to establish
outbound connection to port 25 over IPv4 and IPv4 and uses a validating
DNS resolver.
