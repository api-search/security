---
api_specs:
- filename: kannkidas-de-openapi.yml
  format: yaml
  label: Kann KI das? API
  slug: kann-ki-das-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kannkidas-de/refs/heads/main/openapi/kannkidas-de-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: kannkidas.de
  spf: false
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: kannkidas.de
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kannkidas De Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kann KI das? Sponsoring Agent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Kann KI das? Sponsoring Agent
provider_slug: kannkidas-de
slug: kannkidas-de-domain-security
source_filename: kannkidas-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kannkidas.de\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kannkidas.de\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kannkidas-de/refs/heads/main/security/kannkidas-de-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC
tags:
- Company
- Sponsoring
- Advertising
- Software Reviews
- Build vs Buy
- Search
- agent-native
- MCP
- A2A
- Authentication
- x402
- Stripe Checkout
- Germany
---
