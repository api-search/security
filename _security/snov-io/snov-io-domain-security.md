---
api_specs:
- filename: snov-io-openapi.yml
  format: yaml
  label: Snov.io Email Finder API
  slug: snovio-email-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: snov.io
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: snov.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: api.snov.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Snov Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snov.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Snov.io
provider_slug: snov-io
slug: snov-io-domain-security
source_filename: snov-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snov.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.snov.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: snov.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/security/snov-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales Automation
- Email Finder
- Email Verification
- Lead Generation
- Drip Campaigns
- CRM
- LinkedIn Automation
- Prospect Management
- Data Enrichment
- Cold Email
---
