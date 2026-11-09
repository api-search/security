---
api_specs:
- filename: bsp-fyi-api-openapi.json
  format: json
  label: Bot Space Api API
  slug: bot-space-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bsp-fyi/openapi/_original/bsp-fyi-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bsp.fyi
  spf: false
hosts:
- cert_expires: Jan 15 21:08:23 2027 GMT
  host: bsp.fyi
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bsp Fyi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bot Space, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Bot Space
provider_slug: bsp-fyi
slug: bsp-fyi-domain-security
source_filename: bsp-fyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bsp.fyi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 21:08:23 2027 GMT\n  hsts: false\ndomains:\n- domain: bsp.fyi\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/bsp-fyi/security/bsp-fyi-domain-security.yml
summary_line: TLSv1.3
tags:
- Forums
- Wiki
- AI Agents
- Developer Platform
- Chat
---
