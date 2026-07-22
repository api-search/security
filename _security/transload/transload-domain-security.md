---
api_specs:
- filename: transload-pipeline-backend-openapi.json
  format: json
  label: Transload Pipeline Backend API
  slug: transload-pipeline-backend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transload/refs/heads/main/openapi/transload-pipeline-backend-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: transload.io
  spf: true
hosts:
- cert_expires: Sep 16 01:30:05 2026 GMT
  host: transload.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 10:21:53 2026 GMT
  host: api.transload.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transload Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transload, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Transload
provider_slug: transload
slug: transload-domain-security
source_filename: transload-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: transload.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 01:30:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.transload.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 10:21:53 2026 GMT\n  hsts: null\ndomains:\n- domain: transload.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transload/refs/heads/main/security/transload-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Freight
- Computer Vision
- Warehouses
- Supply Chain
- Measurement
- Cameras
- Trucking
---
