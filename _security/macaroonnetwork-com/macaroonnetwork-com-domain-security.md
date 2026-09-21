---
api_specs:
- filename: macaroonnetwork-com-openapi.json
  format: json
  label: Macaroon Network Agent Services API
  slug: agent-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macaroonnetwork-com/refs/heads/main/openapi/macaroonnetwork-com-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: macaroonnetwork.com
  spf: true
hosts:
- cert_expires: Nov  1 20:54:50 2026 GMT
  host: macaroonnetwork.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 20:54:50 2026 GMT
  host: api.macaroonnetwork.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Macaroonnetwork Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Macaroon Network, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Macaroon Network
provider_slug: macaroonnetwork-com
slug: macaroonnetwork-com-domain-security
source_filename: macaroonnetwork-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: macaroonnetwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 20:54:50 2026 GMT\n  hsts: false\n- host: api.macaroonnetwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 20:54:50 2026 GMT\n  hsts: null\ndomains:\n- domain: macaroonnetwork.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macaroonnetwork-com/refs/heads/main/security/macaroonnetwork-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Agents
- Agentic Commerce
- A2A
- MCP
- x402
- Data Marketplace
- Compliance
- Sanctions Screening
- Company Data
- Scientific Computing
- Bible
- United Kingdom
- agent-native
---
