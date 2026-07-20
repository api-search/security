---
api_specs:
- filename: alpic-openapi-original.json
  format: json
  label: Alpic API
  slug: alpic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/openapi/alpic-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: alpic.ai
  spf: true
hosts:
- cert_expires: Oct  4 10:57:23 2026 GMT
  host: alpic.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: api.alpic.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alpic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alpic, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Alpic
provider_slug: alpic
slug: alpic-domain-security
source_filename: alpic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alpic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 10:57:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.alpic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: alpic.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/security/alpic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai/Ml
- MCP
- Model Context Protocol
- Cloud Platform
- Developer Tools
- Deployment
- ChatGPT Apps
- Agentic
---
