---
api_specs:
- filename: nooks-sequencing-openapi.yml
  format: yaml
  label: Nooks Sequencing API
  slug: nooks-sequencing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-sequencing-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nooks.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nooks.in
  spf: true
hosts:
- cert_expires: Nov  6 22:41:01 2026 GMT
  host: www.nooks.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:21:48 2026 GMT
  host: developer.nooks.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 06:47:29 2026 GMT
  host: partner-api.nooks.in
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nooks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nooks, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nooks
provider_slug: nooks
slug: nooks-domain-security
source_filename: nooks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nooks.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 22:41:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.nooks.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:21:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: partner-api.nooks.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 06:47:29 2026 GMT\n  hsts: null\ndomains:\n- domain: nooks.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: nooks.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/security/nooks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Sales Engagement
- Sales Dialer
- AI SDR
- Outbound Sales
- Sales Coaching
- Revenue Operations
- Sales Sequencing
- CRM Integration
- Agents
- MCP
---
