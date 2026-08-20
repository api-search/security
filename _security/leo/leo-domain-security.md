---
api_specs:
- filename: leo-prospects-api-openapi.yml
  format: yaml
  label: LeO Public API
  slug: leo-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leo/refs/heads/main/openapi/leo-prospects-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: meetleo.com
  spf: true
hosts:
- cert_expires: Nov 11 21:24:30 2026 GMT
  host: www.meetleo.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: api.meetleo.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_note: The automated probe recorded null because it reads the header from a 200 on /; this host returns 404 at the root. Corrected from a direct header read of GET https://api.meetleo.com/health (2026-08-14).
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: mcp.meetleo.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_note: Same correction; read directly from GET https://mcp.meetleo.com/health (2026-08-14).
  hsts_preload: true
  https: true
  security_headers:
  - 'x-frame-options: DENY'
  - 'x-content-type-options: nosniff'
  - 'referrer-policy: strict-origin-when-cross-origin'
  - 'x-xss-protection: 1; mode=block'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LeO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LeO
provider_slug: leo
slug: leo-domain-security
source_filename: leo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meetleo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 21:24:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.meetleo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  hsts_note: >-\n    The automated probe recorded null because it reads the header from a 200 on /;\n    this host returns 404 at the root. Corrected from a direct header read of\n    GET https://api.meetleo.com/health (2026-08-14).\n- host: mcp.meetleo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  hsts_note: >-\n    Same correction; read directly from GET https://mcp.meetleo.com/health\n \
  \   (2026-08-14).\n  security_headers:\n  - 'x-frame-options: DENY'\n  - 'x-content-type-options: nosniff'\n  - 'referrer-policy: strict-origin-when-cross-origin'\n  - 'x-xss-protection: 1; mode=block'\ndomains:\n- domain: meetleo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leo/refs/heads/main/security/leo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Commercial Insurance
- Property and Casualty
- Employee Benefits
- Insurtech
- Artificial Intelligence
- Sales
- Lead Generation
- Prospecting
- Data Enrichment
- Sales Intelligence
- Non-Profit
- Trucking
- MCP
- agent-native
---
