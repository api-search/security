---
api_specs:
- filename: greenhelix-net-a2a-commerce-gateway-openapi.yml
  format: yaml
  label: A2A Commerce Gateway API
  slug: a2a-commerce-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhelix-net/refs/heads/main/openapi/greenhelix-net-a2a-commerce-gateway-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: greenhelix.net
  spf: true
hosts:
- cert_expires: Oct 21 02:25:35 2026 GMT
  host: greenhelix.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 02:25:35 2026 GMT
  host: api.greenhelix.net
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 02:25:35 2026 GMT
  host: sandbox.greenhelix.net
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Greenhelix Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Green Helix, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Green Helix
provider_slug: greenhelix-net
slug: greenhelix-net-domain-security
source_filename: greenhelix-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: greenhelix.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 02:25:35 2026 GMT\n  hsts: false\n- host: api.greenhelix.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 02:25:35 2026 GMT\n  hsts: null\n- host: sandbox.greenhelix.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 02:25:35 2026 GMT\n  hsts: null\ndomains:\n- domain: greenhelix.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greenhelix-net/refs/heads/main/security/greenhelix-net-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Agents
- Agentic Commerce
- Payments
- Escrow
- Billing
- Marketplace
- Identity
- Trust
- Messaging
- Webhook
- MCP
- A2A
- x402
---
