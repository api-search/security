---
api_specs:
- filename: millimetric-openapi.yml
  format: yaml
  label: Millimetric Analytics API
  slug: millimetric-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/millimetric/refs/heads/main/openapi/millimetric-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  dmarc: false
  dnssec: false
  domain: millimetric.ai
  spf: true
hosts:
- cert_expires: Oct 16 03:45:17 2026 GMT
  host: millimetric.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 22:14:38 2026 GMT
  host: api.millimetric.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Millimetric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Millimetric, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Millimetric
provider_slug: millimetric
slug: millimetric-domain-security
source_filename: millimetric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: millimetric.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 03:45:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.millimetric.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 22:14:38 2026 GMT\n  hsts: null\ndomains:\n- domain: millimetric.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/millimetric/refs/heads/main/security/millimetric-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Analytics
- Web Analytics
- Product Analytics
- Attribution
- Privacy
- MCP
- AI Agents
- Events
- Developer Tools
---
