---
api_specs:
- filename: anysphere-cursor-ai-originservice-api-openapi.yml
  format: yaml
  label: Anysphere Cursor Ai Origin Service API
  slug: anysphere-cursor-ai-originservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anysphere-cursor-ai/refs/heads/main/openapi/anysphere-cursor-ai-originservice-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cursor.com
  spf: true
hosts:
- cert_expires: Nov 24 11:10:16 2026 GMT
  host: cursor.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  4 23:59:59 2027 GMT
  host: api.cursor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Anysphere Cursor Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anysphere Cursor Ai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Anysphere Cursor Ai
provider_slug: anysphere-cursor-ai
slug: anysphere-cursor-ai-domain-security
source_filename: anysphere-cursor-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cursor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 11:10:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cursor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  4 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: cursor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anysphere-cursor-ai/refs/heads/main/security/anysphere-cursor-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Coding
- Developer-Tools
- Automation
- Platform
---
