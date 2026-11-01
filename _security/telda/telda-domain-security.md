---
api_specs:
- filename: telda-openapi-generated.yml
  format: yaml
  label: Telda API
  slug: telda-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/telda/openapi/_ae-authored/telda-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: telda.app
  spf: true
hosts:
- cert_expires: Jan  6 03:37:51 2027 GMT
  host: telda.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Telda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Telda, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Telda
provider_slug: telda
slug: telda-domain-security
source_filename: telda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: telda.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 03:37:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: telda.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/telda/security/telda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- MobileApp
- DigitalBanking
---
