---
api_specs:
- filename: ledge-api-openapi.yml
  format: yaml
  label: Ledge API
  slug: ledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledge/refs/heads/main/openapi/ledge-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ledge.co
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: goledge.io
  spf: false
hosts:
- cert_expires: Sep  5 02:40:20 2026 GMT
  host: www.ledge.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: api.goledge.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: 'The generic probe of / returns 404 without the HSTS header; probing the documented API path GET /v1/api/{orgId}/sources returns HTTP 401 with `strict-transport-security: max-age=31536000; includeSubDomains; preload`. Recorded from that observed response.'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ledge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ledge, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ledge
provider_slug: ledge
slug: ledge-domain-security
source_filename: ledge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ledge.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 02:40:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.goledge.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: >-\n    The generic probe of / returns 404 without the HSTS header; probing the\n    documented API path GET /v1/api/{orgId}/sources returns HTTP 401 with\n    `strict-transport-security: max-age=31536000; includeSubDomains; preload`.\n    Recorded from that observed response.\ndomains:\n- domain: ledge.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: goledge.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ledge/refs/heads/main/security/ledge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Accounting
- Reconciliation
- Financial Close
- Payment Operations
- Transaction Matching
- Cash Application
- Journal Entries
- AI Agents
- ERP Integration
- Finance Automation
---
