---
api_specs:
- filename: api-docs.json
  format: json
  label: Cambio Uruguay API
  slug: cambio-uruguay-api
  spec_type: OpenAPI
  url: https://api.cambio-uruguay.com/api-docs.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cambio-uruguay.com
  spf: true
hosts:
- cert_expires: Oct 13 17:07:06 2026 GMT
  host: cambio-uruguay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 17:07:06 2026 GMT
  host: api.cambio-uruguay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Cambio Uruguay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cambio Uruguay, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cambio Uruguay
provider_slug: cambio-uruguay
slug: cambio-uruguay-domain-security
source_filename: cambio-uruguay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cambio-uruguay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 17:07:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cambio-uruguay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 17:07:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cambio-uruguay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cambio-uruguay/refs/heads/main/security/cambio-uruguay-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Currency
- Exchange Rates
- Finance
- Uruguay
- Latin America
- MCP
- agent-native
- Open Source
---
