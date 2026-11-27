---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coolant.run
  spf: false
hosts:
- cert_expires: Feb  2 18:46:21 2027 GMT
  host: coolant.run
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coolant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coolant, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Coolant
provider_slug: coolant-run
slug: coolant-run-domain-security
source_filename: coolant-run-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coolant.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 18:46:21 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coolant.run\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/coolant-run/security/coolant-run-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- MCP
- x402
- Agent Tools
- Micropayments
- Developer Utilities
---
