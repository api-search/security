---
api_specs:
- filename: tray-ai-embedded-api-openapi.yml
  format: yaml
  label: Tray.ai Embedded API
  slug: embedded-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-embedded-api-openapi.yml
- filename: tray-ai-platform-api-openapi.yml
  format: yaml
  label: Tray.ai Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-platform-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tray.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tray.io
  spf: true
hosts:
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: tray.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: tray.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: api.tray.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tray Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tray.ai, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tray.ai
provider_slug: tray-ai
slug: tray-ai-domain-security
source_filename: tray-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tray.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: tray.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.tray.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tray.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tray.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/security/tray-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- Integration
- iPaaS
- AI Agents
- MCP
---
