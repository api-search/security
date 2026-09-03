---
api_specs:
- filename: medblocks-platform-openapi.json
  format: json
  label: Medblocks Platform API
  slug: medblocks-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medblocks/refs/heads/main/openapi/medblocks-platform-openapi.json
- filename: medblocks-public-site-openapi.json
  format: json
  label: Medblocks Public Site API
  slug: medblocks-public-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medblocks/refs/heads/main/openapi/medblocks-public-site-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: medblocks.com
  spf: true
hosts:
- cert_expires: Nov 24 22:04:24 2026 GMT
  host: medblocks.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 17:22:39 2026 GMT
  host: app.medblocks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Medblocks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Medblocks, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Medblocks
provider_slug: medblocks
slug: medblocks-domain-security
source_filename: medblocks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: medblocks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 22:04:24 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: app.medblocks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 17:22:39 2026 GMT\n  hsts: false\ndomains:\n- domain: medblocks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medblocks/refs/heads/main/security/medblocks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- Healthcare
- FHIR
- openEHR
- Interoperability
- Electronic Health Records
- Patient Access
- Health Data
- SMART on FHIR
- Webhooks
- Model Context Protocol
- Company
---
