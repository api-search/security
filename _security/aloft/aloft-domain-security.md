---
api_specs:
- filename: aloft-openapi-original.json
  format: json
  label: Aloft API V1
  slug: aloft-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aloft/refs/heads/main/openapi/aloft-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aloft.ai
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: www.aloft.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: api.aloft.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aloft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aloft, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aloft
provider_slug: aloft
slug: aloft-domain-security
source_filename: aloft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aloft.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: false\n- host: api.aloft.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: aloft.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aloft/refs/heads/main/security/aloft-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Drones
- Airspace
- UTM
- LAANC
- Aviation
- Fleet Management
- Geospatial
- Public Safety
---
