# check_mx_all_flavours

[![markdownlint](https://github.com/andreasschulze/check_mx_all_flavours/actions/workflows/markdownlint.yml/badge.svg)](https://github.com/andreasschulze/check_mx_all_flavours/actions/workflows/markdownlint.yml)
[![shellcheck](https://github.com/andreasschulze/check_mx_all_flavours/actions/workflows/shellcheck.yml/badge.svg)](https://github.com/andreasschulze/check_mx_all_flavours/actions/workflows/shellcheck.yml)

## Usage

```sh
check_mx_all_flavours <domain>
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

## Requirements

The following tools must be available in \$PATH:

* awk
* dig or kdig
* ldns-dane
* openssl
* sed
* sleep

## Author

Andreas Schulze
