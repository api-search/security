---
api_specs:
- filename: snowsignals-daas-openapi.json
  format: json
  label: SnowSignals API
  slug: snowsignals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowsignals/refs/heads/main/openapi/snowsignals-daas-openapi.json
- filename: snowsignals-x402-openapi.json
  format: json
  label: SnowSignals x402 Gateway
  slug: snowsignals-x402-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowsignals/refs/heads/main/openapi/snowsignals-x402-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: snowsignals.io
  spf: true
hosts:
- cert_expires: Dec  8 13:56:48 2026 GMT
  host: snowsignals.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Snowsignals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SnowSignals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SnowSignals
provider_slug: snowsignals
slug: snowsignals-domain-security
source_filename: snowsignals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snowsignals.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 13:56:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: snowsignals.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snowsignals/refs/heads/main/security/snowsignals-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- crypto
- market-data
- bitcoin
- analytics
- market-phase
- regime
- trendvane
- daas
- mcp
- agent-native
- financial-data
- x402
---
