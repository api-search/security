---
api_specs:
- filename: quadrant-api-openapi.json
  format: json
  label: Quadrant API
  slug: quadrant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quadrant-api/main/openapi/quadrant-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: qis.io
  spf: true
hosts:
- cert_expires: Nov 10 18:42:18 2026 GMT
  host: api.qis.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quadrant Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quadrant API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Quadrant API
provider_slug: quadrant-api
slug: quadrant-api-domain-security
source_filename: quadrant-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.qis.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 18:42:18 2026 GMT\n  hsts: null\ndomains:\n- domain: qis.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quadrant-api/refs/heads/main/security/quadrant-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Alerts
- Security
- Threat Intelligence
---
