---
api_specs:
- filename: mono-co-account-information-api-openapi.yml
  format: yaml
  label: Mono Account Information API
  slug: mono-co-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-account-information-api-openapi.yml
- filename: mono-co-account-linking-api-openapi.yml
  format: yaml
  label: Mono Account Linking API
  slug: mono-co-account-linking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-account-linking-api-openapi.yml
- filename: mono-co-direct-debit-api-openapi.yml
  format: yaml
  label: Mono Direct Debit API
  slug: mono-co-direct-debit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-direct-debit-api-openapi.yml
- filename: mono-co-directpay-api-openapi.yml
  format: yaml
  label: Mono DirectPay API
  slug: mono-co-directpay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-directpay-api-openapi.yml
- filename: mono-co-identity-and-income-api-openapi.yml
  format: yaml
  label: Mono Identity and Income API
  slug: mono-co-identity-and-income-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-identity-and-income-api-openapi.yml
- filename: mono-co-transactions-and-statements-api-openapi.yml
  format: yaml
  label: Mono Transactions and Statements API
  slug: mono-co-transactions-and-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-transactions-and-statements-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mono.co
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: withmono.com
  spf: false
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: mono.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: docs.mono.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: api.withmono.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mono Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mono, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mono
provider_slug: mono-co
slug: mono-co-domain-security
source_filename: mono-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mono.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: false\n- host: docs.mono.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: false\n- host: api.withmono.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: mono.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: withmono.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/security/mono-co-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Open Banking
- Financial Data
- Payments
- Direct Debit
- Africa
---
