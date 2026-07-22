---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: varada.io
  mx: false
  nameservers:
  - ns1-coming-soon.sav.com
  - ns2-coming-soon.sav.com
  parked: true
  spf: false
hosts:
- host: varada.io
  hsts: false
  https: false
  https_error: SSLCertVerificationError (certificate verify failed)
  port_80_open: true
- host: www.varada.io
  https: false
  https_error: connection failed (curl exit 92, HTTP 000)
kind: domain-security
layout: security
method: probed
name: Varada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Varada, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Varada
provider_slug: varada
slug: varada-domain-security
source_filename: varada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: dig + TLS probe of varada.io (enrichment pipeline, manual probe run)\nnote: >-\n  Varada was acquired by Starburst Data in June 2022 and the varada.io domain is\n  no longer operated by the company: nameservers point at ns1/ns2-coming-soon.sav.com\n  (a domain-marketplace parking service). HTTPS fails certificate verification and\n  port 80 serves an empty response. All records below are what was actually observed\n  on 2026-07-21 — absence is valid data.\nhosts:\n  - host: varada.io\n    https: false\n    https_error: SSLCertVerificationError (certificate verify failed)\n    port_80_open: true\n    hsts: false\n  - host: www.varada.io\n    https: false\n    https_error: connection failed (curl exit 92, HTTP 000)\ndomains:\n  - domain: varada.io\n    nameservers:\n      - ns1-coming-soon.sav.com\n      - ns2-coming-soon.sav.com\n    parked: true\n    dnssec: false\n    caa: []\n    spf: false\n    dmarc: false\n    mx: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/varada/refs/heads/main/security/varada-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Data
- Data Lakes
- Analytics
- Trino
- Presto
- Query Acceleration
- Acquired
---
