---
api_specs:
- filename: candor-money-conversations-api-openapi.yml
  format: yaml
  label: Candor Finance Conversations API
  slug: candor-money-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/candor-money/openapi/candor-money-conversations-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: candor.money
  spf: false
hosts:
- cert_expires: Dec  1 23:12:42 2026 GMT
  host: candor.money
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Candor Money Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Candor Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Candor Finance
provider_slug: candor-money
slug: candor-money-domain-security
source_filename: candor-money-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: candor.money\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:12:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: candor.money\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/candor-money/security/candor-money-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Finance
- AI
- PersonalFinance
- Budgeting
---
