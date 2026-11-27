---
api_specs:
- filename: leanscale-team-access-api-openapi.yml
  format: yaml
  label: LeanScale Access API
  slug: leanscale-team-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leanscale-team/openapi/leanscale-team-access-api-openapi.yml
- filename: leanscale-team-mcp-api-openapi.yml
  format: yaml
  label: LeanScale MCP API
  slug: leanscale-team-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leanscale-team/openapi/leanscale-team-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leanscale.team
  spf: true
hosts:
- cert_expires: Jan 15 08:49:10 2027 GMT
  host: leanscale.team
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LeanScale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LeanScale, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LeanScale
provider_slug: leanscale-team
slug: leanscale-team-domain-security
source_filename: leanscale-team-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leanscale.team\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 08:49:10 2027 GMT\n  hsts: false\ndomains:\n- domain: leanscale.team\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/leanscale-team/security/leanscale-team-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Go-To-Market
- Revenue Operations
- Software-as-a-Service
- AI-native
- Consulting
---
