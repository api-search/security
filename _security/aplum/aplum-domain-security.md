---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: aplum.com
  ds_records: []
  mx:
  - aspmx.l.google.com
  nameservers:
  - vip3.alidns.com
  - vip4.alidns.com
  spf: false
hosts:
- host: aplum.com
  hsts: null
  hsts_max_age: null
  https: null
  reachable: false
  reachable_note: connection refused/timeout from probe location (geo-restricted host)
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Aplum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aplum, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: aplum
provider_slug: aplum
slug: aplum-domain-security
source_filename: aplum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: dig DNS records for aplum.com; HTTPS/TLS host unreachable from probe location\nnotes: >-\n  aplum.com is a China-hosted consumer platform (resolves to\n  wan.slb04.zhuanzhuan.com / 49.233.247.241). HTTPS/TLS/HSTS could not be\n  measured from the probe location (connection refused / timeout). DNS-level\n  records below were resolved successfully and absence of a record is valid,\n  recorded data. Nameservers are Alibaba Cloud DNS (alidns.com); mail is on\n  Google Workspace (aspmx.l.google.com).\nhosts:\n  - host: aplum.com\n    https: null\n    tls_version: null\n    hsts: null\n    hsts_max_age: null\n    reachable: false\n    reachable_note: connection refused/timeout from probe location (geo-restricted host)\ndomains:\n  - domain: aplum.com\n    dnssec: false\n    ds_records: []\n    caa: []\n    spf: false\n    dmarc: false\n    dmarc_policy: null\n    nameservers:\n      - vip3.alidns.com\n      - vip4.alidns.com\n    mx:\n\
  \      - aspmx.l.google.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aplum/refs/heads/main/security/aplum-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Second-Hand
- Luxury Fashion
- Resale Marketplace
- E-Commerce
- Consumer
- China
---
