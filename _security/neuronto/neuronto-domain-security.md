---
api_specs:
- filename: neuronto-openapi.json
  format: json
  label: Neuronto ARD Registry API
  slug: ard-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neuronto/refs/heads/main/openapi/neuronto-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: neuronto.com
  spf: true
hosts:
- cert_expires: Nov  6 03:35:58 2026 GMT
  host: neuronto.com
  hsts: max-age=31536000; includeSubDomains
  hsts_note: Observed live on https://neuronto.com/stats response headers 2026-09-07 (strict-transport-security); the automated probe recorded null on the homepage fetch.
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Neuronto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neuronto ARD Registry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Neuronto ARD Registry
provider_slug: neuronto
slug: neuronto-domain-security
source_filename: neuronto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: neuronto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 03:35:58 2026 GMT\n  hsts: 'max-age=31536000; includeSubDomains'\n  hsts_note: Observed live on https://neuronto.com/stats response headers 2026-09-07\n    (strict-transport-security); the automated probe recorded null on the homepage\n    fetch.\ndomains:\n- domain: neuronto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neuronto/refs/heads/main/security/neuronto-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Agentic Resource Discovery
- ARD
- MCP
- A2A
- API Discovery
- Registry
---
