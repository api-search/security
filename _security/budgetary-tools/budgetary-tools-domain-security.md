---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: budgetary.tools
  spf: true
hosts:
- cert_expires: Jan 13 02:38:19 2027 GMT
  host: budgetary.tools
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Budgetary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Budgetary, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Budgetary
provider_slug: budgetary-tools
slug: budgetary-tools-domain-security
source_filename: budgetary-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: budgetary.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 02:38:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: budgetary.tools\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/budgetary-tools/security/budgetary-tools-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- AI Coding
- MCP Server
- Free Tier
---
