---
api_specs:
- filename: fin-authentication-api-openapi.yml
  format: yaml
  label: Fin Authentication API
  slug: fin-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fin/refs/heads/main/openapi/fin-authentication-api-openapi.yml
- filename: fin-balances-api-openapi.yml
  format: yaml
  label: Fin Balances API
  slug: fin-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fin/refs/heads/main/openapi/fin-balances-api-openapi.yml
- filename: fin-beneficiaries-api-openapi.yml
  format: yaml
  label: Fin Beneficiaries API
  slug: fin-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fin/refs/heads/main/openapi/fin-beneficiaries-api-openapi.yml
- filename: fin-catalogue-api-openapi.yml
  format: yaml
  label: Fin Catalogue API
  slug: fin-catalogue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fin/refs/heads/main/openapi/fin-catalogue-api-openapi.yml
- filename: fin-crypto-orchestration-api-openapi.yml
  format: yaml
  label: Fin Crypto Orchestration API
  slug: fin-crypto-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fin/refs/heads/main/openapi/fin-crypto-orchestration-api-openapi.yml
- filename: fin-customers-api-openapi.yml
  format: yaml
  label: Fin Customers API
  slug: fin-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fin/refs/heads/main/openapi/fin-customers-api-openapi.yml
- filename: fin-fees-fx-rates-api-openapi.yml
  format: yaml
  label: Fin Fees & FX Rates API
  slug: fin-fees-fx-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fin/refs/heads/main/openapi/fin-fees-fx-rates-api-openapi.yml
- filename: fin-transactions-api-openapi.yml
  format: yaml
  label: Fin Transactions API
  slug: fin-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fin/refs/heads/main/openapi/fin-transactions-api-openapi.yml
- filename: fin-virtual-accounts-api-openapi.yml
  format: yaml
  label: Fin Virtual Accounts API
  slug: fin-virtual-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fin/refs/heads/main/openapi/fin-virtual-accounts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fin.com
  spf: true
hosts:
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: www.fin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: sandbox.api.fin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: api.fin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fin, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fin
provider_slug: fin
slug: fin-domain-security
source_filename: fin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: false\n- host: sandbox.api.fin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: null\n- host: api.fin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fin/refs/heads/main/security/fin-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Cross-Border Payments
- Stablecoins
- Fintech
- Money Movement
- Foreign Exchange
- Virtual Accounts
- Crypto
---
