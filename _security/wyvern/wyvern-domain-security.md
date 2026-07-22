---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wyvern.space
  spf: true
hosts:
- cert_expires: Sep 13 21:13:31 2026 GMT
  host: wyvern.space
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 15:34:19 2026 GMT
  host: archive.wyvern.space
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 22:38:18 2026 GMT
  host: opendata.wyvern.space
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wyvern Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wyvern, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wyvern
provider_slug: wyvern
slug: wyvern-domain-security
source_filename: wyvern-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wyvern.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 21:13:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: archive.wyvern.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 15:34:19 2026 GMT\n  hsts: false\n- host: opendata.wyvern.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 22:38:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: wyvern.space\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wyvern/refs/heads/main/security/wyvern-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Space
- Earth Observation
- Hyperspectral Imaging
- Satellites
- Geospatial
- Remote Sensing
- Open Data
- Agriculture
---
