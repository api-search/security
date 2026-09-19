---
api_specs:
- filename: assetfare-auth-api-openapi.yml
  format: yaml
  label: AssetFare Auth API
  slug: assetfare-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-auth-api-openapi.yml
- filename: assetfare-quote-api-openapi.yml
  format: yaml
  label: AssetFare Quote API
  slug: assetfare-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-quote-api-openapi.yml
- filename: assetfare-session-api-openapi.yml
  format: yaml
  label: AssetFare Session API
  slug: assetfare-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-session-api-openapi.yml
- filename: assetfare-status-api-openapi.yml
  format: yaml
  label: AssetFare Status API
  slug: assetfare-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-status-api-openapi.yml
- filename: assetfare-well-known-api-openapi.yml
  format: yaml
  label: AssetFare .well Known API
  slug: assetfare-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: assetfare.dev
  spf: true
hosts:
- cert_expires: Dec 13 01:33:34 2026 GMT
  host: assetfare.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 01:46:12 2026 GMT
  host: api.assetfare.dev
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Assetfare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AssetFare, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AssetFare
provider_slug: assetfare
slug: assetfare-domain-security
source_filename: assetfare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: assetfare.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 01:33:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.assetfare.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 01:46:12 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: assetfare.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/security/assetfare-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI Agents
- Asset Transfer
- Bridge
- Cross-Chain
- Non-Custodial
- Cryptocurrency
- Solana
- Base
- OpenAPI
- MCP
- Agent Skills
---
