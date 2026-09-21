---
api_specs:
- filename: agentum-lat-apis-brasil-openapi.json
  format: json
  label: AGENTUM APIs Brasil
  slug: apis-brasil
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentum-lat/refs/heads/main/openapi/agentum-lat-apis-brasil-openapi.json
- filename: agentum-lat-business-openapi.json
  format: json
  label: AGENTUM Business API
  slug: business
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentum-lat/refs/heads/main/openapi/agentum-lat-business-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agentum.lat
  spf: true
hosts:
- cert_expires: Nov 29 22:07:26 2026 GMT
  host: agentum.lat
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 22:08:53 2026 GMT
  host: business.agentum.lat
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Agentum Lat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AGENTUM, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AGENTUM
provider_slug: agentum-lat
slug: agentum-lat-domain-security
source_filename: agentum-lat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentum.lat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 22:07:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: business.agentum.lat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 22:08:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agentum.lat\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentum-lat/refs/heads/main/security/agentum-lat-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Business Intelligence
- KYB
- Company Data
- Compliance
- Brazil
- x402
- Agentic Commerce
- Exchange Rates
- Address Verification
- Economic Data
- MCP
- A2A
- Agents
---
