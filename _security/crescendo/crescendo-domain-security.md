---
api_specs:
- filename: crescendo-platform-openapi-original.json
  format: json
  label: Crescendo Platform API
  slug: crescendo-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crescendo/refs/heads/main/openapi/crescendo-platform-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crescendo.ai
  spf: true
hosts:
- cert_expires: Oct 16 12:40:35 2026 GMT
  host: platform.crescendo.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crescendo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crescendo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Crescendo
provider_slug: crescendo
slug: crescendo-domain-security
source_filename: crescendo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: platform.crescendo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 12:40:35 2026 GMT\n  hsts: false\ndomains:\n- domain: crescendo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crescendo/refs/heads/main/security/crescendo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Customer Experience
- Customer Support
- Artificial Intelligence
- AI Agents
- Contact Center
- Conversational AI
- Voice of Customer
- MCP
---
