---
api_specs:
- filename: bridgestackapi-openapi-generated.yml
  format: yaml
  label: BridgeStackAPI API
  slug: bridgestackapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridgestackapi/refs/heads/main/openapi/_ae-authored/bridgestackapi-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bridgestackapi.com
  spf: true
hosts:
- cert_expires: Dec 13 14:08:41 2026 GMT
  host: bridgestackapi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bridgestackapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BridgeStackAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BridgeStackAPI
provider_slug: bridgestackapi
slug: bridgestackapi-domain-security
source_filename: bridgestackapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bridgestackapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 14:08:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bridgestackapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bridgestackapi/refs/heads/main/security/bridgestackapi-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- API Gateway
- Usage Control
- B2B SaaS
- External APIs
---
