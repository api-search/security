---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: data.eco
  mx: true
  mx_provider: google-workspace
  spf: false
  txt_records:
  - qqdlt7bphj94c74fsruincgj6i
  - lnf67bhbglklqvpgdjhaag4evs
hosts:
- cert_expiry: null
  host: data.eco
  hsts: null
  hsts_max_age: null
  https: false
  ip: 47.75.45.50
  reachable: false
  tls_version: null
- cert_expiry: null
  host: docs.data.eco
  hsts: null
  hsts_max_age: null
  https: false
  ip: 47.75.153.56
  reachable: false
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Data, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Data
provider_slug: data
slug: data-domain-security
source_filename: data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: dig (DNS) + TLS/HTTP HEAD probe\nnote: >-\n  Public hosts for data.eco (Alibaba Cloud IPs) did not accept TLS/HTTP\n  connections from this vantage point (connection timeout / refused on 443) at\n  probe time, so HTTPS reachability, TLS version, cert expiry, and HSTS could not\n  be observed. DNS-level facts below are real and complete. Absence of a record\n  (no CAA, no SPF, no DMARC policy, no DNSSEC) is recorded as observed data, not\n  a probe failure.\nhosts:\n  - host: data.eco\n    ip: 47.75.45.50\n    https: false\n    reachable: false\n    tls_version: null\n    cert_expiry: null\n    hsts: null\n    hsts_max_age: null\n  - host: docs.data.eco\n    ip: 47.75.153.56\n    https: false\n    reachable: false\n    tls_version: null\n    cert_expiry: null\n    hsts: null\n    hsts_max_age: null\ndomains:\n  - domain: data.eco\n    dnssec: false\n    caa: []\n    spf: false\n    dmarc: false\n    dmarc_policy: null\n    mx:\
  \ true\n    mx_provider: google-workspace\n    txt_records:\n      - \"qqdlt7bphj94c74fsruincgj6i\"\n      - \"lnf67bhbglklqvpgdjhaag4evs\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data/refs/heads/main/security/data-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Crypto
---
