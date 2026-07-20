---
api_specs:
- filename: boom-ai-openapi-original.json
  format: json
  label: Boom API
  slug: boom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/openapi/boom-ai-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: useboom.ai
  spf: true
hosts:
- cert_expires: Sep  6 17:45:51 2026 GMT
  host: docs.useboom.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 23:45:17 2026 GMT
  host: www.useboom.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 18:59:10 2026 GMT
  host: dev.useboom.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boom Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boom Ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Boom Ai
provider_slug: boom-ai
slug: boom-ai-domain-security
source_filename: boom-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.useboom.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 17:45:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.useboom.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 23:45:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dev.useboom.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 18:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: useboom.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/security/boom-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Conversational AI
- Customer Engagement
- Customer Data Platform
- Messaging
- WhatsApp
- SMS
- Marketing Automation
- E-commerce
- Agents
- MCP
---
