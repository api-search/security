---
api_specs:
- filename: temp-md-openapi.yml
  format: yaml
  label: temp.md Public API
  slug: tempmd-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temp-md/refs/heads/main/openapi/temp-md-openapi.yml
- filename: temp-md-platform-openapi.yml
  format: yaml
  label: temp.md Embedded Preview Platform API
  slug: tempmd-embedded-preview-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temp-md/refs/heads/main/openapi/temp-md-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: temp.md
  spf: true
hosts:
- cert_expires: Oct 31 07:01:29 2026 GMT
  host: temp.md
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 04:42:57 2026 GMT
  host: api.temp.md
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Temp Md Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for temp.md, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: temp.md
provider_slug: temp-md
slug: temp-md-domain-security
source_filename: temp-md-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: temp.md\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 07:01:29 2026 GMT\n  hsts: false\n- host: api.temp.md\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 04:42:57 2026 GMT\n  hsts: null\ndomains:\n- domain: temp.md\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temp-md/refs/heads/main/security/temp-md-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Web Publishing
- Static Hosting
- AI Agents
- MCP
- A2A
- Developer Tools
- Preview Infrastructure
- File Sharing
- Agent-Native
- Company
---
