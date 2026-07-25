---
api_specs:
- filename: fastforex-admin-api-openapi.yml
  format: yaml
  label: FastForex admin API
  slug: fastforex-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastforex/refs/heads/main/openapi/fastforex-admin-api-openapi.yml
- filename: fastforex-crypto-api-openapi.yml
  format: yaml
  label: FastForex crypto API
  slug: fastforex-crypto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastforex/refs/heads/main/openapi/fastforex-crypto-api-openapi.yml
- filename: fastforex-currency-api-openapi.yml
  format: yaml
  label: FastForex currency API
  slug: fastforex-currency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastforex/refs/heads/main/openapi/fastforex-currency-api-openapi.yml
- filename: fastforex-fx-api-openapi.yml
  format: yaml
  label: FastForex fx API
  slug: fastforex-fx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastforex/refs/heads/main/openapi/fastforex-fx-api-openapi.yml
- filename: fastforex-plan-extra-api-openapi.yml
  format: yaml
  label: FastForex plan-extra API
  slug: fastforex-plan-extra-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastforex/refs/heads/main/openapi/fastforex-plan-extra-api-openapi.yml
- filename: fastforex-plan-one-api-openapi.yml
  format: yaml
  label: FastForex plan-one API
  slug: fastforex-plan-one-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastforex/refs/heads/main/openapi/fastforex-plan-one-api-openapi.yml
- filename: fastforex-plan-premium-api-openapi.yml
  format: yaml
  label: FastForex plan-premium API
  slug: fastforex-plan-premium-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastforex/refs/heads/main/openapi/fastforex-plan-premium-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fastforex.io
  spf: true
hosts:
- cert_expires: Sep 29 15:59:34 2026 GMT
  host: www.fastforex.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 04:11:48 2026 GMT
  host: api.fastforex.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:55:10 2026 GMT
  host: api.beta.fastforex.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fastforex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FastForex, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FastForex
provider_slug: fastforex
slug: fastforex-domain-security
source_filename: fastforex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fastforex.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 15:59:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fastforex.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 04:11:48 2026 GMT\n  hsts: null\n- host: api.beta.fastforex.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:55:10 2026 GMT\n  hsts: null\ndomains:\n- domain: fastforex.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fastforex/refs/heads/main/security/fastforex-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Currency Exchange
- Forex
- Financial Data
- Exchange Rates
- Cryptocurrency
- FX Trading
- Historical Data
- Real-Time Data
---
