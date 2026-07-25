---
api_specs:
- filename: moov-accounts-api-openapi.yml
  format: yaml
  label: Moov Accounts API
  slug: moov-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-accounts-api-openapi.yml
- filename: moov-authentication-api-openapi.yml
  format: yaml
  label: Moov Authentication API
  slug: moov-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-authentication-api-openapi.yml
- filename: moov-bank-accounts-api-openapi.yml
  format: yaml
  label: Moov Bank Accounts API
  slug: moov-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-bank-accounts-api-openapi.yml
- filename: moov-capabilities-api-openapi.yml
  format: yaml
  label: Moov Capabilities API
  slug: moov-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-capabilities-api-openapi.yml
- filename: moov-cards-api-openapi.yml
  format: yaml
  label: Moov Cards API
  slug: moov-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-cards-api-openapi.yml
- filename: moov-disputes-api-openapi.yml
  format: yaml
  label: Moov Disputes API
  slug: moov-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-disputes-api-openapi.yml
- filename: moov-payment-links-api-openapi.yml
  format: yaml
  label: Moov Payment Links API
  slug: moov-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-payment-links-api-openapi.yml
- filename: moov-payment-methods-api-openapi.yml
  format: yaml
  label: Moov Payment Methods API
  slug: moov-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-payment-methods-api-openapi.yml
- filename: moov-refunds-api-openapi.yml
  format: yaml
  label: Moov Refunds API
  slug: moov-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-refunds-api-openapi.yml
- filename: moov-representatives-api-openapi.yml
  format: yaml
  label: Moov Representatives API
  slug: moov-representatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-representatives-api-openapi.yml
- filename: moov-sweeps-api-openapi.yml
  format: yaml
  label: Moov Sweeps API
  slug: moov-sweeps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-sweeps-api-openapi.yml
- filename: moov-transfers-api-openapi.yml
  format: yaml
  label: Moov Transfers API
  slug: moov-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-transfers-api-openapi.yml
- filename: moov-wallets-api-openapi.yml
  format: yaml
  label: Moov Wallets API
  slug: moov-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-wallets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moov.io
  spf: true
hosts:
- cert_expires: Oct  6 21:33:43 2026 GMT
  host: docs.moov.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 18:49:20 2026 GMT
  host: moov.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: api.moov.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moov, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Moov
provider_slug: moov
slug: moov-domain-security
source_filename: moov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.moov.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:33:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: moov.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 18:49:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.moov.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: moov.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/security/moov-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Embedded Finance
- Financial Infrastructure
- Money Movement
- Payments
- Transfers
---
