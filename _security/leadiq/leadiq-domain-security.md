---
api_specs:
- filename: leadiq-data-api-openapi.yml
  format: yaml
  label: LeadIQ Data API
  slug: leadiq-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadiq/refs/heads/main/openapi/leadiq-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: leadiq.com
  spf: true
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: leadiq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: developer.leadiq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: api.leadiq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leadiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LeadIQ, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: LeadIQ
provider_slug: leadiq
slug: leadiq-domain-security
source_filename: leadiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leadiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.leadiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: false\n- host: api.leadiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: leadiq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leadiq/refs/heads/main/security/leadiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Sales Intelligence
- B2B Data
- Contact Data
- Lead Generation
- Prospecting
- CRM Enrichment
- Sales Engagement
- GraphQL
- Model Context Protocol
- Revenue Operations
- Go To Market
---
