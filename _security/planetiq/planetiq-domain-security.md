---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: planetiq.com
  spf: true
hosts:
- cert_expires: Oct 11 16:01:39 2026 GMT
  host: planetiq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Planetiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PlanetiQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PlanetiQ
provider_slug: planetiq
slug: planetiq-domain-security
source_filename: planetiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: planetiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 16:01:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: planetiq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planetiq/refs/heads/main/security/planetiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Weather
- Satellite
- Earth Observation
- Space Weather
- Atmospheric Data
- GNSS Radio Occultation
- Climate
- Aerospace
- Defense
- Geospatial
---
