---
api_specs:
- filename: humanforai-dev-api-openapi.json
  format: json
  label: Human For AI API API
  slug: human-for-ai-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/humanforai-dev/openapi/_original/humanforai-dev-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: humanforai.dev
  spf: false
hosts:
- cert_expires: Jan 28 16:00:00 2027 GMT
  host: humanforai.dev
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Human For AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Human For AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Human For AI
provider_slug: humanforai-dev
slug: humanforai-dev-domain-security
source_filename: humanforai-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: humanforai.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 16:00:00 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: humanforai.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/humanforai-dev/security/humanforai-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Human-in-the-Loop
- Verification
- Services
---
