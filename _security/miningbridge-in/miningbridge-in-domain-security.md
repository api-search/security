---
api_specs:
- filename: miningbridge-in-openapi.json
  format: json
  label: MiningBridge API
  slug: miningbridge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/miningbridge-in/openapi/miningbridge-in-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: miningbridge.in
  spf: true
hosts:
- cert_expires: Jan 19 06:06:49 2027 GMT
  host: miningbridge.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MiningBridge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MiningBridge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MiningBridge
provider_slug: miningbridge-in
slug: miningbridge-in-domain-security
source_filename: miningbridge-in-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: miningbridge.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 06:06:49 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: miningbridge.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/miningbridge-in/security/miningbridge-in-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Critical Minerals
- Artificial Intelligence
- Data Platform
- Supply Chain
---
