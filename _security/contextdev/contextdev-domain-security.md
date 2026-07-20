---
api_specs:
- filename: contextdev-openapi.yml
  format: yaml
  label: Context API
  slug: context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextdev/refs/heads/main/openapi/contextdev-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: context.dev
  spf: true
hosts:
- cert_expires: Oct  9 19:25:05 2026 GMT
  host: api.context.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Contextdev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Context.dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Context.dev
provider_slug: contextdev
slug: contextdev-domain-security
source_filename: contextdev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.context.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 19:25:05 2026 GMT\n  hsts: null\ndomains:\n- domain: context.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contextdev/refs/heads/main/security/contextdev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Web Scraping
- Brand Intelligence
- Data Enrichment
- AI Agents
- Web Data
- Classification
- Website Monitoring
- Company Data
- Developer Tools
- APIs
---
