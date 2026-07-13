---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iceye.com
  spf: true
hosts:
- cert_expires: Oct  5 03:21:18 2026 GMT
  host: www.iceye.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: docs.iceye.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.iceye.com
  https: false
kind: domain-security
layout: security
method: probed
name: Iceye Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ICEYE, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ICEYE
provider_slug: iceye
slug: iceye-domain-security
source_filename: iceye-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iceye.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 03:21:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.iceye.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.iceye.com\n  https: false\ndomains:\n- domain: iceye.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iceye/refs/heads/main/security/iceye-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SAR
- Satellite Imagery
- Earth Observation
- Tasking
- Catalog
- Flood Monitoring
- Disaster Response
- Defense
- ISR
- Geospatial
- All-Weather
---
