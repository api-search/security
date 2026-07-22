---
api_specs:
- filename: process-street-openapi-original.json
  format: json
  label: Process Street Public API
  slug: process-street-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/process-street/refs/heads/main/openapi/process-street-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: process.st
  spf: true
hosts:
- cert_expires: Oct  9 09:13:25 2026 GMT
  host: www.process.st
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: public-api.process.st
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Process Street Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Process Street, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Process Street
provider_slug: process-street
slug: process-street-domain-security
source_filename: process-street-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.process.st\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 09:13:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public-api.process.st\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: process.st\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/process-street/refs/heads/main/security/process-street-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Productivity
- Workflow
- Workflow Automation
- Process Management
- No-Code
- Business Process
- Task Management
- SaaS
- MCP
---
