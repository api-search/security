---
api_specs:
- filename: lane-api-openapi.yml
  format: yaml
  label: Lane API
  slug: lane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lane-api/refs/heads/main/openapi/lane-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: netsolapp.io
  spf: true
hosts:
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: docs.netsolapp.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lane Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lane API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lane API
provider_slug: lane-api
slug: lane-api-domain-security
source_filename: lane-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.netsolapp.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: netsolapp.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lane-api/refs/heads/main/security/lane-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Asset Leasing
- Credit
- Loans
---
