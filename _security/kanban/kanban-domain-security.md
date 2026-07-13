---
api_specs:
- filename: kanban-openapi.yml
  format: yaml
  label: Kanban Tool REST API v3
  slug: kanban-tool-rest-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanban/refs/heads/main/openapi/kanban-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kanbantool.com
  spf: true
hosts:
- cert_expires: Aug 15 10:16:07 2026 GMT
  host: kanbantool.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- host: your_domain.kanbantool.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''your_domain'
kind: domain-security
layout: security
method: probed
name: Kanban Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kanban Tool, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kanban Tool
provider_slug: kanban
slug: kanban-domain-security
source_filename: kanban-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kanbantool.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 10:16:07 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: your_domain.kanbantool.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''your_domain'\n  hsts: null\ndomains:\n- domain: kanbantool.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kanban/refs/heads/main/security/kanban-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agile
- Boards
- Kanban
- Project Management
- Task Management
- Time Tracking
- Workflow
---
