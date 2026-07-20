---
api_specs:
- filename: gumloop-openapi-original.yml
  format: yaml
  label: Gumloop Public API
  slug: gumloop-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gumloop.com
  spf: true
hosts:
- cert_expires: Aug 25 22:36:22 2026 GMT
  host: www.gumloop.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 03:30:54 2026 GMT
  host: api.gumloop.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gumloop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gumloop, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gumloop
provider_slug: gumloop
slug: gumloop-domain-security
source_filename: gumloop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gumloop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 22:36:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.gumloop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:30:54 2026 GMT\n  hsts: null\ndomains:\n- domain: gumloop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/security/gumloop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Automation
- Workflow Automation
- Agent Platform
- MCP
- LLM
- No-Code
- Developer Tools
---
