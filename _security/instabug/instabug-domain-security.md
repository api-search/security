---
api_specs:
- filename: instabug-mcp-server-openapi.yml
  format: yaml
  label: Luciq MCP Server
  slug: mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instabug/refs/heads/main/openapi/instabug-mcp-server-openapi.yml
- filename: instabug-webhooks-asyncapi.yml
  format: yaml
  label: Luciq Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/instabug/refs/heads/main/asyncapi/instabug-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: luciq.ai
  spf: true
hosts:
- cert_expires: Sep 21 01:12:14 2026 GMT
  host: luciq.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 14:27:25 2026 GMT
  host: docs.luciq.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: api.luciq.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Instabug Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instabug (Luciq), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Instabug (Luciq)
provider_slug: instabug
slug: instabug-domain-security
source_filename: instabug-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: luciq.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 01:12:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.luciq.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 14:27:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.luciq.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: luciq.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instabug/refs/heads/main/security/instabug-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agentic AI
- APM
- Application Performance Monitoring
- Bug Reporting
- Crash Reporting
- MCP
- Mobile
- Mobile Observability
- Observability
- Session Replay
---
