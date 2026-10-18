---
api_specs:
- filename: mcpnest-openapi-generated.yml
  format: yaml
  label: MCPNest API
  slug: mcpnest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcpnest/refs/heads/main/openapi/_ae-authored/mcpnest-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mcpnest.io
  spf: false
hosts:
- cert_expires: Jan  5 03:57:40 2027 GMT
  host: mcpnest.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mcpnest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MCPNest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: MCPNest
provider_slug: mcpnest
slug: mcpnest-domain-security
source_filename: mcpnest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcpnest.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 03:57:40 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mcpnest.io\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mcpnest/refs/heads/main/security/mcpnest-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cloud
- DevOps
- AI
---
