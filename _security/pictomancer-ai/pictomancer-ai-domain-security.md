---
api_specs:
- filename: pictomancer-ai-openapi.yml
  format: yaml
  label: Pictomancer.ai Image API
  slug: pictomancer-ai-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pictomancer-ai/refs/heads/main/openapi/pictomancer-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: pictomancer.ai
  spf: false
hosts:
- cert_expires: Nov 10 01:49:20 2026 GMT
  host: pictomancer.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 00:03:18 2026 GMT
  host: api.pictomancer.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Pictomancer Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pictomancer.ai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Pictomancer.ai
provider_slug: pictomancer-ai
slug: pictomancer-ai-domain-security
source_filename: pictomancer-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pictomancer.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 01:49:20 2026 GMT\n  hsts: false\n- host: api.pictomancer.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 00:03:18 2026 GMT\n  hsts: null\ndomains:\n- domain: pictomancer.ai\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pictomancer-ai/refs/heads/main/security/pictomancer-ai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Image
- Image Optimization
- Image Processing
- Media
- Agents
- MCP
- A2A
- x402
- Micropayments
- Developer Tools
---
