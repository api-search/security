---
api_specs:
- filename: honeygate-app-openapi-generated.yml
  format: yaml
  label: HoneyGate API
  slug: honeygate-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honeygate-app/openapi/_ae-authored/honeygate-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: honeygate.app
  spf: false
hosts:
- cert_expires: Dec 29 03:07:51 2026 GMT
  host: honeygate.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HoneyGate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HoneyGate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: HoneyGate
provider_slug: honeygate-app
slug: honeygate-app-domain-security
source_filename: honeygate-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: honeygate.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 03:07:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: honeygate.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/honeygate-app/security/honeygate-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Bot
- Discord
- Community
- Automation
---
