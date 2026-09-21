---
api_specs:
- filename: horizonshield-dev-mcp-conduct-register-openapi.json
  format: json
  label: MCP Verification Gate (MCP conduct register) API
  slug: mcp-verification-gate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizonshield-dev/refs/heads/main/openapi/horizonshield-dev-mcp-conduct-register-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: the-horizons-innovation.com
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: horizonshield.dev
  spf: false
hosts:
- cert_expires: Oct 22 05:06:19 2026 GMT
  host: shield.the-horizons-innovation.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 00:43:44 2026 GMT
  host: mcp.horizonshield.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 00:43:44 2026 GMT
  host: gate.horizonshield.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Horizonshield Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The HORIZ音s株式会社, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: The HORIZ音s株式会社
provider_slug: horizonshield-dev
slug: horizonshield-dev-domain-security
source_filename: horizonshield-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shield.the-horizons-innovation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 05:06:19 2026 GMT\n  hsts: false\n- host: mcp.horizonshield.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 00:43:44 2026 GMT\n  hsts: null\n- host: gate.horizonshield.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 00:43:44 2026 GMT\n  hsts: null\ndomains:\n- domain: the-horizons-innovation.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: horizonshield.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/horizonshield-dev/refs/heads/main/security/horizonshield-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Construction
- Renovation
- Cost Estimation
- Fair Pricing
- Consumer Protection
- Verification
- Transparency Ledger
- Open Data
- MCP
- A2A
- AP2
- Agents
- agent-native
- Japan
---
