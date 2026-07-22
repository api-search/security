---
api_specs:
- filename: pixxel-openapi-original.json
  format: json
  label: Pixxel API (stargate)
  slug: pixxel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/openapi/pixxel-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pixxel.space
  spf: true
hosts:
- cert_expires: Aug  2 01:20:42 2026 GMT
  host: pixxel.space
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: api.pixxel.space
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pixxel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pixxel, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pixxel
provider_slug: pixxel
slug: pixxel-domain-security
source_filename: pixxel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pixxel.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  2 01:20:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pixxel.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: pixxel.space\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixxel/refs/heads/main/security/pixxel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Satellite Imagery
- Earth Observation
- Hyperspectral
- Geospatial
- Remote Sensing
- Analytics
- STAC
---
