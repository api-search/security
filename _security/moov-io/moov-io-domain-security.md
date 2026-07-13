---
api_specs:
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Accounts API
  slug: moov-io-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Representatives API
  slug: moov-io-representatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Capabilities API
  slug: moov-io-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Underwriting API
  slug: moov-io-underwriting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Bank Accounts API
  slug: moov-io-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Cards API
  slug: moov-io-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Wallets API
  slug: moov-io-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Payment Methods API
  slug: moov-io-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Transfers API
  slug: moov-io-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Refunds API
  slug: moov-io-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Sweeps API
  slug: moov-io-sweeps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Disputes API
  slug: moov-io-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Card Issuing API
  slug: moov-io-card-issuing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Institutions API
  slug: moov-io-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moov.io
  spf: true
hosts:
- cert_expires: Oct  7 18:49:20 2026 GMT
  host: moov.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 21:33:43 2026 GMT
  host: docs.moov.io
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
name: Moov Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moov, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Moov
provider_slug: moov-io
slug: moov-io-domain-security
source_filename: moov-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moov.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 18:49:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.moov.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:33:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.moov.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: moov.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/security/moov-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Money Movement
- Fintech
- ACH
- RTP
- Cards
- Wallets
- Embedded Finance
---
