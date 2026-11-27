---
api_specs:
- filename: merx-exchange-payments-api-openapi.yml
  format: yaml
  label: MERX Payments API
  slug: merx-exchange-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merx-exchange/openapi/merx-exchange-payments-api-openapi.yml
- filename: merx-exchange-tron-api-openapi.yml
  format: yaml
  label: MERX TRON API
  slug: merx-exchange-tron-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merx-exchange/openapi/merx-exchange-tron-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: merx.exchange
  spf: true
hosts:
- cert_expires: Jan 13 13:44:14 2027 GMT
  host: merx.exchange
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MERX Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MERX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MERX
provider_slug: merx-exchange
slug: merx-exchange-domain-security
source_filename: merx-exchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: merx.exchange\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 13:44:14 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: merx.exchange\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/merx-exchange/security/merx-exchange-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Energy
- Blockchain
- Payments
- Automation
- Artificial Intelligence
---
