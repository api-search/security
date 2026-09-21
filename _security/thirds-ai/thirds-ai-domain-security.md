---
api_specs:
- filename: thirds-ai-openapi.yml
  format: yaml
  label: thirds.ai REST API
  slug: thirdsai-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirds-ai/refs/heads/main/openapi/thirds-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thirds.ai
  spf: true
hosts:
- cert_expires: Oct 28 23:15:09 2026 GMT
  host: thirds.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Thirds Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for thirds.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: thirds.ai
provider_slug: thirds-ai
slug: thirds-ai-domain-security
source_filename: thirds-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thirds.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:15:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thirds.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thirds-ai/refs/heads/main/security/thirds-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- pdf-automation
- image-automation
- Document Generation
- HTML to PDF
- HTML to Image
- template-rendering
- Branded Content
- Developer Tools
- MCP Server
- agent-native
- marketing-ops
---
