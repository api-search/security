---
api_specs:
- filename: context7-openapi.yml
  format: yaml
  label: Context7 REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/context7/refs/heads/main/openapi/context7-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: context7.com
  spf: true
hosts:
- cert_expires: Aug 26 06:50:31 2026 GMT
  host: context7.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: mcp.context7.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Context7 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Context7, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Context7
provider_slug: context7
slug: context7-domain-security
source_filename: context7-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: context7.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 06:50:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: mcp.context7.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: context7.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/context7/refs/heads/main/security/context7-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI
- Context
- Documentation
- LLM
- MCP
---
