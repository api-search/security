---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: wutwut.com
  mx: []
  nameservers:
  - ns1.emailverification.info
  - ns2.emailverification.info
  spf: false
hosts:
- host: wutwut.com
  hsts: false
  http_note: registrar suspension page (nginx/1.18.0 Ubuntu), catch-all for all paths
  http_status: 200
  https: false
  https_error: connection refused (port 443)
  ip: 94.23.162.163
  tls_version: null
- host: www.wutwut.com
  http_status: 200
  https: false
  https_error: connection refused (port 443)
  ip: 94.23.162.163
kind: domain-security
layout: security
method: probed
name: Wutwut Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for wutwut, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: wutwut
provider_slug: wutwut
slug: wutwut-domain-security
source_filename: wutwut-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: probe (curl + dig) of wutwut.com; probe-domain-security.py reported host unreachable over HTTPS\nnote: >-\n  wutwut.com is a suspended/parked domain. HTTPS (port 443) refuses connections;\n  HTTP serves a Key-Systems GmbH registrar \"ICANN contact verification suspension\"\n  page (Last-Modified 2021-04-08) as a catch-all for every path. The DNS zone is\n  delegated to the registrar's suspension nameservers (ns1/ns2.emailverification.info).\n  Absence of records below is real probed data.\nhosts:\n  - host: wutwut.com\n    ip: 94.23.162.163\n    https: false\n    https_error: connection refused (port 443)\n    http_status: 200\n    http_note: registrar suspension page (nginx/1.18.0 Ubuntu), catch-all for all paths\n    tls_version: null\n    hsts: false\n  - host: www.wutwut.com\n    ip: 94.23.162.163\n    https: false\n    https_error: connection refused (port 443)\n    http_status: 200\ndomains:\n  - domain: wutwut.com\n  \
  \  nameservers: [ns1.emailverification.info, ns2.emailverification.info]\n    dnssec: false\n    caa: []\n    spf: false\n    dmarc: false\n    dmarc_policy: null\n    mx: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wutwut/refs/heads/main/security/wutwut-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Startup
- Venture Portfolio
- Slow Ventures
- Inactive
---
