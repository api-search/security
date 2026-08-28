---
api_specs:
- filename: pvcase-anderson-optimization-openapi.json
  format: json
  label: PVcase Prospect API (Anderson Optimization API)
  slug: pvcase-prospect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pvcase/refs/heads/main/openapi/pvcase-anderson-optimization-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pvcase.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gitbook.io
  spf: true
hosts:
- cert_expires: Oct  1 15:07:38 2026 GMT
  host: pvcase.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 19:03:12 2026 GMT
  host: pvcase-prospect.gitbook.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: core-v1.carbon.prod.andersonopt.com
  https: false
kind: domain-security
layout: security
method: probed
name: Pvcase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PVcase, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PVcase
provider_slug: pvcase
slug: pvcase-domain-security
source_filename: pvcase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pvcase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 15:07:38 2026 GMT\n  hsts: false\n- host: pvcase-prospect.gitbook.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 19:03:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: core-v1.carbon.prod.andersonopt.com\n  https: false\ndomains:\n- domain: pvcase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gitbook.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pvcase/refs/heads/main/security/pvcase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Solar
- Energy
- Renewable Energy
- Photovoltaic
- Geospatial
- Site Selection
- Engineering Design
- Simulation
- Project Development
- CAD
---
