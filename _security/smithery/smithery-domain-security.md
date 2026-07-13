---
api_specs:
- filename: smithery-openapi.json
  format: json
  label: Smithery Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery/refs/heads/main/openapi/smithery-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: smithery.ai
  spf: true
hosts:
- cert_expires: Sep 23 15:19:05 2026 GMT
  host: smithery.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 07:31:52 2026 GMT
  host: api.smithery.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smithery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smithery, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Smithery
provider_slug: smithery
slug: smithery-domain-security
source_filename: smithery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smithery.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 15:19:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.smithery.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 07:31:52 2026 GMT\n  hsts: null\ndomains:\n- domain: smithery.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smithery/refs/heads/main/security/smithery-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Large Language Models
- MCP
- Model Context Protocol
- AI Agents
- Developer Tools
- Registry
- Skills
- Tool Discovery
---
