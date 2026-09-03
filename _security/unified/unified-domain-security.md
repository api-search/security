---
api_specs:
- filename: unified-mcp-service-openapi.json
  format: json
  label: Unified MCP Service
  slug: unified-mcp-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified/refs/heads/main/openapi/unified-mcp-service-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: unified.com
  spf: true
hosts:
- cert_expires: Oct 15 07:03:43 2026 GMT
  host: www.unified.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: api.unified.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unified Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unified, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Unified
provider_slug: unified
slug: unified-domain-security
source_filename: unified-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unified.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 07:03:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.unified.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: unified.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unified/refs/heads/main/security/unified-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Advertising
- Social Media
- Digital Advertising
- Marketing
- Analytics
- Media
- Agents
- MCP
---
