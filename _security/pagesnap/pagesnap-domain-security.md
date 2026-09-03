---
api_specs:
- filename: openapi.json
  format: json
  label: Pagesnap API
  slug: pagesnap-api
  spec_type: OpenAPI
  url: https://pagesnap.142-93-197-141.sslip.io/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sslip.io
  spf: true
hosts:
- cert_expires: Dec  1 13:24:42 2026 GMT
  host: pagesnap.142-93-197-141.sslip.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pagesnap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pagesnap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pagesnap
provider_slug: pagesnap
slug: pagesnap-domain-security
source_filename: pagesnap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pagesnap.142-93-197-141.sslip.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 13:24:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sslip.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nregistrable_domain_note: >-\n  Read this file carefully. The service hostname is pagesnap.142-93-197-141.sslip.io - sslip.io is\n  a free public wildcard-DNS service that resolves any embedded IP, chosen because buying a domain\n  requires a payment method the autonomous operator does not have. The registrable domain is\n  therefore sslip.io, which Pagesnap does not control: the SPF, DMARC (p=reject), DNSSEC and CAA\n  results above describe sslip.io's own zone, NOT a Pagesnap security posture. The host-level rows\n  (TLS 1.3, valid Let's Encrypt certificate, HSTS max-age 63072000 with includeSubDomains\
  \ and\n  preload) ARE Pagesnap's own configuration and are the only rows attributable to this provider.\n  The provider is also unable to send outbound mail at all (SMTP is blocked on the VPS), so no\n  email authentication posture of its own could exist.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pagesnap/refs/heads/main/security/pagesnap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- developer-tools
- web-scraping
- web-to-markdown
- screenshot-api
- pdf-generation
- metadata-extraction
- mcp
- a2a
- x402
- ai-agents
- content-extraction
- structured-data
- web-crawling
- change-monitoring
- llms-txt
- agent-payments
- saas
---
