---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: capellaspace.com
  spf: true
hosts:
- cert_expires: Aug 28 14:15:24 2026 GMT
  host: www.capellaspace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 13:20:36 2026 GMT
  host: docs.capellaspace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: api.capellaspace.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Capella Space Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capella Space, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Capella Space
provider_slug: capella-space
slug: capella-space-domain-security
source_filename: capella-space-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.capellaspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 14:15:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.capellaspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 13:20:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.capellaspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: capellaspace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capella-space/refs/heads/main/security/capella-space-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Synthetic Aperture Radar
- SAR
- Earth Observation
- Satellite Imagery
- Geospatial
- STAC
- Remote Sensing
- Tasking
- Catalog
---
