---
api_specs:
- filename: notbank-openapi-generated.yml
  format: yaml
  label: Notbank API
  slug: notbank-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notbank/openapi/_ae-authored/notbank-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: notbank.com
  spf: true
hosts:
- cert_expires: Jan  8 10:28:31 2027 GMT
  host: notbank.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Notbank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Notbank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Notbank
provider_slug: notbank
slug: notbank-domain-security
source_filename: notbank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: notbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 10:28:31 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: notbank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/notbank/security/notbank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Cryptocurrency
- Fintech
- Digital Assets
---
