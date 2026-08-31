---
api_specs:
- filename: fipto-aisp-pisp-api-openapi.yml
  format: yaml
  label: Fipto AISP/PISP API
  slug: fipto-aisp-pisp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-aisp-pisp-api-openapi.yml
- filename: fipto-assets-api-openapi.yml
  format: yaml
  label: Fipto Assets API
  slug: fipto-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-assets-api-openapi.yml
- filename: fipto-automations-api-openapi.yml
  format: yaml
  label: Fipto Automations API
  slug: fipto-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-automations-api-openapi.yml
- filename: fipto-beneficiaries-api-openapi.yml
  format: yaml
  label: Fipto Beneficiaries API
  slug: fipto-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-beneficiaries-api-openapi.yml
- filename: fipto-companies-api-openapi.yml
  format: yaml
  label: Fipto Companies API
  slug: fipto-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-companies-api-openapi.yml
- filename: fipto-conversions-api-openapi.yml
  format: yaml
  label: Fipto Conversions API
  slug: fipto-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-conversions-api-openapi.yml
- filename: fipto-internal-transfers-api-openapi.yml
  format: yaml
  label: Fipto Internal Transfers API
  slug: fipto-internal-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-internal-transfers-api-openapi.yml
- filename: fipto-payin-simulation-api-openapi.yml
  format: yaml
  label: Fipto Payin Simulation API
  slug: fipto-payin-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-payin-simulation-api-openapi.yml
- filename: fipto-payment-links-api-openapi.yml
  format: yaml
  label: Fipto Payment links API
  slug: fipto-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-payment-links-api-openapi.yml
- filename: fipto-transactions-api-openapi.yml
  format: yaml
  label: Fipto Transactions API
  slug: fipto-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-transactions-api-openapi.yml
- filename: fipto-travel-rule-api-openapi.yml
  format: yaml
  label: Fipto Travel Rule API
  slug: fipto-travel-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-travel-rule-api-openapi.yml
- filename: fipto-wallets-api-openapi.yml
  format: yaml
  label: Fipto Wallets API
  slug: fipto-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-wallets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fipto.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fipto.app
  spf: true
hosts:
- cert_expires: Nov  9 04:52:31 2026 GMT
  host: fipto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 13:06:19 2026 GMT
  host: docs.fipto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: api.fipto.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fipto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fipto, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Fipto
provider_slug: fipto
slug: fipto-domain-security
source_filename: fipto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fipto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 04:52:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.fipto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 13:06:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fipto.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: fipto.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fipto.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/security/fipto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Blockchain
- Payments
- Stablecoins
- Banking
- Treasury
- Cross-Border Payments
- Digital Currency
- Fintech
- Wallets
---
