---
api_specs:
- filename: drippay-openapi-original.json
  format: json
  label: Drip API
  slug: drip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drippay/refs/heads/main/openapi/drippay-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: usedrip.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: drippay.dev
  spf: true
hosts:
- cert_expires: Oct 13 20:13:34 2026 GMT
  host: docs.usedrip.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 22:00:36 2026 GMT
  host: api.drippay.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Drippay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drippay, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Drippay
provider_slug: drippay
slug: drippay-domain-security
source_filename: drippay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.usedrip.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 20:13:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.drippay.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 22:00:36 2026 GMT\n  hsts: null\ndomains:\n- domain: usedrip.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: drippay.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drippay/refs/heads/main/security/drippay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Billing
- Usage-Based Billing
- Metering
- Monetization
- Payments
- AI Agents
- Developer Tools
- Webhooks
- MCP
- CRM
- Sales Automation
---
