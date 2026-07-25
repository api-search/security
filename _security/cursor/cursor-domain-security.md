---
api_specs:
- filename: cursor-audit-logs-api-openapi.yml
  format: yaml
  label: Cursor Audit Logs API
  slug: cursor-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/openapi/cursor-audit-logs-api-openapi.yml
- filename: cursor-groups-api-openapi.yml
  format: yaml
  label: Cursor Groups API
  slug: cursor-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/openapi/cursor-groups-api-openapi.yml
- filename: cursor-members-api-openapi.yml
  format: yaml
  label: Cursor Members API
  slug: cursor-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/openapi/cursor-members-api-openapi.yml
- filename: cursor-repo-blocklists-api-openapi.yml
  format: yaml
  label: Cursor Repo Blocklists API
  slug: cursor-repo-blocklists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/openapi/cursor-repo-blocklists-api-openapi.yml
- filename: cursor-spend-api-openapi.yml
  format: yaml
  label: Cursor Spend API
  slug: cursor-spend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/openapi/cursor-spend-api-openapi.yml
- filename: cursor-usage-api-openapi.yml
  format: yaml
  label: Cursor Usage API
  slug: cursor-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/openapi/cursor-usage-api-openapi.yml
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
