---
api_specs:
- filename: arroway-app-mcp.json
  format: json
  label: Arroway MCP API
  slug: arroway-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arroway-app/openapi/arroway-app-mcp.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arroway.app
  spf: true
hosts:
- cert_expires: Dec 29 05:14:58 2026 GMT
  host: arroway.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arroway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arroway, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Arroway
provider_slug: arroway-app
slug: arroway-app-domain-security
source_filename: arroway-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arroway.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 05:14:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: arroway.app\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/arroway-app/security/arroway-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Collaboration
- Memory
- Teamwork
- Automation
---
