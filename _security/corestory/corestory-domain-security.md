---
api_specs:
- filename: corestory-openapi-original.json
  format: json
  label: CoreStory API
  slug: corestory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corestory/refs/heads/main/openapi/corestory-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: corestory.ai
  spf: true
hosts:
- cert_expires: Sep 19 06:00:48 2026 GMT
  host: corestory.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Corestory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoreStory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CoreStory
provider_slug: corestory
slug: corestory-domain-security
source_filename: corestory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corestory.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 06:00:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: corestory.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corestory/refs/heads/main/security/corestory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Code Intelligence
- Legacy Modernization
- Developer Tools
- Code Analysis
- Documentation
- MCP
- Agentic
---
