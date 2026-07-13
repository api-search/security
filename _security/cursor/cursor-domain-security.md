---
api_specs:
- filename: cursor-admin-api-openapi.yml
  format: yaml
  label: Cursor Admin API
  slug: admin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/openapi/cursor-admin-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cursor.com
  spf: true
hosts:
- cert_expires: Sep 22 12:25:03 2026 GMT
  host: cursor.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: api.cursor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cursor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cursor, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cursor
provider_slug: cursor
slug: cursor-domain-security
source_filename: cursor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cursor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 12:25:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cursor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: cursor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/security/cursor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Developer Tools
- Code Editor
- Agent
- IDE
- Cloud Agents
---
