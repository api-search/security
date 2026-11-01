---
api_specs:
- filename: bankbridge-money-openapi-generated.yml
  format: yaml
  label: BankBridge API
  slug: bankbridge-money-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankbridge-money/openapi/_ae-authored/bankbridge-money-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bankbridge.money
  spf: false
hosts:
- cert_expires: Jan 20 22:11:16 2027 GMT
  host: bankbridge.money
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bankbridge Money Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BankBridge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: BankBridge
provider_slug: bankbridge-money
slug: bankbridge-money-domain-security
source_filename: bankbridge-money-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bankbridge.money\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 22:11:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bankbridge.money\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bankbridge-money/security/bankbridge-money-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Finance
- AI
- MCP
- Banking
---
