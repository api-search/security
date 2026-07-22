---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: beelinebikes.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: beelineconnect.com
  spf: true
hosts:
- cert_expires: Oct  9 23:42:07 2026 GMT
  host: beelinebikes.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:42:07 2026 GMT
  host: beelineconnect.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beeline Bikes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beeline Bikes, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Beeline Bikes
provider_slug: beeline-bikes
slug: beeline-bikes-domain-security
source_filename: beeline-bikes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beelinebikes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:42:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: beelineconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:42:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: beelinebikes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: beelineconnect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beeline-bikes/refs/heads/main/security/beeline-bikes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Bicycle
- Retail
- Marketplace
- Scheduling
- Inventory
- Warranty
- Logistics
---
