---
api_specs:
- filename: puzzle-openapi-original.json
  format: json
  label: Puzzle Accounting API
  slug: puzzle-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: puzzle.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Sep 10 13:33:15 2026 GMT
  host: puzzle.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: puzzle-api.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 15:46:04 2026 GMT
  host: api.puzzle.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Puzzle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Puzzle, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Puzzle
provider_slug: puzzle
slug: puzzle-domain-security
source_filename: puzzle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: puzzle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 13:33:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: puzzle-api.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.puzzle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 15:46:04 2026 GMT\n  hsts: null\ndomains:\n- domain: puzzle.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/security/puzzle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Accounting
- Financial
- Bookkeeping
- Fintech
- General Ledger
- Payroll
- Agent-Native
- MCP
---
