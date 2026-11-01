---
api_specs:
- filename: banksapi-openapi-generated.yml
  format: yaml
  label: fineconomy API
  slug: banksapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/banksapi/openapi/_ae-authored/banksapi-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "geotrust.com"
  - 0 issuewild "www.digicert.com"
  - 0 issue "geotrust.com"
  - 0 issue "www.digicert.com"
  - 0 issue "buypass.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: banksapi.de
  spf: true
hosts:
- cert_expires: Dec  1 23:08:07 2026 GMT
  host: banksapi.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Banksapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fineconomy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: fineconomy
provider_slug: banksapi
slug: banksapi-domain-security
source_filename: banksapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: banksapi.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:08:07 2026 GMT\n  hsts: false\ndomains:\n- domain: banksapi.de\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"geotrust.com\"\n  - 0 issuewild \"www.digicert.com\"\n  - 0 issue \"geotrust.com\"\n  - 0 issue \"www.digicert.com\"\n  - 0 issue \"buypass.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/banksapi/security/banksapi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Banking
- API
- FinTech
- Payments
- DataAnalytics
---
