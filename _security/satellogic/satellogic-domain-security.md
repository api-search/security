---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: satellogic.com
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: satellogic.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: developers.satellogic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Satellogic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Satellogic, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Satellogic
provider_slug: satellogic
slug: satellogic-domain-security
source_filename: satellogic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: satellogic.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\n- host: developers.satellogic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: satellogic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/satellogic/refs/heads/main/security/satellogic-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Earth Observation
- Satellite Imagery
- Geospatial
- Remote Sensing
- High Resolution
- Sub-Meter Imagery
- Multispectral
- Hyperspectral
- Tasking
- Archive
- Aleph
- NewSat
- Constellation
- Defense and Intelligence
- Energy and Mining
- Insurance
- Climate
---
