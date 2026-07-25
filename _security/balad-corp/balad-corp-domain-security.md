---
api_specs:
- filename: balad-corp-apis-authentication-api-openapi.yml
  format: yaml
  label: BALAD CORP APIs/Authentication API
  slug: balad-corp-apis-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/balad-corp/refs/heads/main/openapi/balad-corp-apis-authentication-api-openapi.yml
- filename: balad-corp-apis-core-balance-api-openapi.yml
  format: yaml
  label: BALAD CORP APIs/Core/Balance API
  slug: balad-corp-apis-core-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/balad-corp/refs/heads/main/openapi/balad-corp-apis-core-balance-api-openapi.yml
- filename: balad-corp-apis-core-exchange-rate-api-openapi.yml
  format: yaml
  label: BALAD CORP APIs/Core/Exchange rate API
  slug: balad-corp-apis-core-exchange-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/balad-corp/refs/heads/main/openapi/balad-corp-apis-core-exchange-rate-api-openapi.yml
- filename: balad-corp-apis-core-secrets-api-openapi.yml
  format: yaml
  label: BALAD CORP APIs/Core/Secrets API
  slug: balad-corp-apis-core-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/balad-corp/refs/heads/main/openapi/balad-corp-apis-core-secrets-api-openapi.yml
- filename: balad-corp-apis-link-lookups-api-openapi.yml
  format: yaml
  label: BALAD CORP APIs/Link/Lookups API
  slug: balad-corp-apis-link-lookups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/balad-corp/refs/heads/main/openapi/balad-corp-apis-link-lookups-api-openapi.yml
- filename: balad-corp-apis-link-reconciliation-api-openapi.yml
  format: yaml
  label: BALAD CORP APIs/Link/Reconciliation API
  slug: balad-corp-apis-link-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/balad-corp/refs/heads/main/openapi/balad-corp-apis-link-reconciliation-api-openapi.yml
- filename: balad-corp-apis-link-transactions-api-openapi.yml
  format: yaml
  label: BALAD CORP APIs/Link/Transactions API
  slug: balad-corp-apis-link-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/balad-corp/refs/heads/main/openapi/balad-corp-apis-link-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: balad.me
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: balad.tech
  spf: false
hosts:
- cert_expires: Dec 31 15:36:13 2026 GMT
  host: balad.me
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 00:03:05 2026 GMT
  host: developers.balad.tech
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Balad Corp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BALAD CORP, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BALAD CORP
provider_slug: balad-corp
slug: balad-corp-domain-security
source_filename: balad-corp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: balad.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 15:36:13 2026 GMT\n  hsts: null\n- host: developers.balad.tech\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 22 00:03:05 2026 GMT\n  hsts: false\ndomains:\n- domain: balad.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: balad.tech\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/balad-corp/refs/heads/main/security/balad-corp-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Payments
- Remittances
- Cross-Border Payments
- Fintech
- Egypt
- Payouts
- Money Transfer
- Banking
- API
---
