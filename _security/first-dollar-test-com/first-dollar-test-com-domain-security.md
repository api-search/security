---
api_specs:
- filename: first-dollar-test-com-api-openapi.json
  format: json
  label: First Dollar Test Api API
  slug: first-dollar-test-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/first-dollar-test-com/openapi/_original/first-dollar-test-com-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: first-dollar-test.com
  spf: false
hosts:
- cert_expires: Apr  3 23:59:59 2027 GMT
  host: first-dollar-test.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: First Dollar Test Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for First Dollar Test, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: First Dollar Test
provider_slug: first-dollar-test-com
slug: first-dollar-test-com-domain-security
source_filename: first-dollar-test-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: first-dollar-test.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: first-dollar-test.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/first-dollar-test-com/security/first-dollar-test-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Wallet
- API
- Beta
- USDC
---
