---
api_specs:
- filename: dealboard-openapi-generated.yml
  format: yaml
  label: Dealboard API
  slug: dealboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealboard/refs/heads/main/openapi/_ae-authored/dealboard-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getdealboard.com
  spf: true
hosts:
- cert_expires: Dec  9 02:50:33 2026 GMT
  host: getdealboard.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dealboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dealboard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Dealboard
provider_slug: dealboard
slug: dealboard-domain-security
source_filename: dealboard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getdealboard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 02:50:33 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: getdealboard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dealboard/refs/heads/main/security/dealboard-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- CRM
- Sales
- API
- AI
- Integration
---
