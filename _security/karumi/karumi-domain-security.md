---
api_specs:
- filename: karumi-analytics-api-openapi.yml
  format: yaml
  label: Karumi Analytics API
  slug: karumi-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karumi/refs/heads/main/openapi/karumi-analytics-api-openapi.yml
- filename: karumi-sessions-api-openapi.yml
  format: yaml
  label: Karumi Sessions API
  slug: karumi-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karumi/refs/heads/main/openapi/karumi-sessions-api-openapi.yml
- filename: karumi-targets-api-openapi.yml
  format: yaml
  label: Karumi Targets API
  slug: karumi-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karumi/refs/heads/main/openapi/karumi-targets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: karumi.ai
  spf: false
hosts:
- cert_expires: Sep 24 15:03:02 2026 GMT
  host: www.karumi.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 03:50:20 2026 GMT
  host: api.karumi.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Karumi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Karumi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Karumi
provider_slug: karumi
slug: karumi-domain-security
source_filename: karumi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.karumi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 15:03:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.karumi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 03:50:20 2026 GMT\n  hsts: null\ndomains:\n- domain: karumi.ai\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karumi/refs/heads/main/security/karumi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI Agents
- Product Demos
- Sales Enablement
- Go-To-Market
- Software-as-a-Service
- Conversational AI
- Video
- Y Combinator
- MCP
- agent-native
- Analytics
- Conversation Intelligence
---
