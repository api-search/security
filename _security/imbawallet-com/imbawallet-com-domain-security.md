---
api_specs:
- filename: imbawallet-com-auth-api-openapi.yml
  format: yaml
  label: imbawallet-com Auth API
  slug: imbawallet-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-auth-api-openapi.yml
- filename: imbawallet-com-balance-api-openapi.yml
  format: yaml
  label: imbawallet-com Balance API
  slug: imbawallet-com-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-balance-api-openapi.yml
- filename: imbawallet-com-cards-api-openapi.yml
  format: yaml
  label: imbawallet-com Cards API
  slug: imbawallet-com-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-cards-api-openapi.yml
- filename: imbawallet-com-catalog-api-openapi.yml
  format: yaml
  label: imbawallet-com Catalog API
  slug: imbawallet-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-catalog-api-openapi.yml
- filename: imbawallet-com-deposit-api-openapi.yml
  format: yaml
  label: imbawallet-com Deposit API
  slug: imbawallet-com-deposit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-deposit-api-openapi.yml
- filename: imbawallet-com-withdrawals-api-openapi.yml
  format: yaml
  label: imbawallet-com Withdrawals API
  slug: imbawallet-com-withdrawals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-withdrawals-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: imbawallet.com
  spf: true
hosts:
- cert_expires: Dec 23 02:37:46 2026 GMT
  host: imbawallet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Imbawallet Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for imbawallet-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: imbawallet-com
provider_slug: imbawallet-com
slug: imbawallet-com-domain-security
source_filename: imbawallet-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imbawallet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 02:37:46 2026 GMT\n  hsts: false\ndomains:\n- domain: imbawallet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/imbawallet-com/security/imbawallet-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- FinTech
- Payments
- Cryptocurrency
- VirtualCards
- Wallet
---
