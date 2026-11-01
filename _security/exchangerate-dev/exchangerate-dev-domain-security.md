---
api_specs:
- filename: exchangerate-dev-account-api-openapi.yml
  format: yaml
  label: exchangerate-dev Account API
  slug: exchangerate-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-account-api-openapi.yml
- filename: exchangerate-dev-consent-api-openapi.yml
  format: yaml
  label: exchangerate-dev Consent API
  slug: exchangerate-dev-consent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-consent-api-openapi.yml
- filename: exchangerate-dev-convert-api-openapi.yml
  format: yaml
  label: exchangerate-dev Convert API
  slug: exchangerate-dev-convert-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-convert-api-openapi.yml
- filename: exchangerate-dev-currencies-api-openapi.yml
  format: yaml
  label: exchangerate-dev Currencies API
  slug: exchangerate-dev-currencies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-currencies-api-openapi.yml
- filename: exchangerate-dev-exchangerate-dev-api-openapi.yml
  format: yaml
  label: exchangerate-dev Exchangerate.dev API
  slug: exchangerate-dev-exchangerate-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-exchangerate-dev-api-openapi.yml
- filename: exchangerate-dev-health-api-openapi.yml
  format: yaml
  label: exchangerate-dev Health API
  slug: exchangerate-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-health-api-openapi.yml
- filename: exchangerate-dev-indices-api-openapi.yml
  format: yaml
  label: exchangerate-dev Indices API
  slug: exchangerate-dev-indices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-indices-api-openapi.yml
- filename: exchangerate-dev-keys-api-openapi.yml
  format: yaml
  label: exchangerate-dev Keys API
  slug: exchangerate-dev-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-keys-api-openapi.yml
- filename: exchangerate-dev-latest-api-openapi.yml
  format: yaml
  label: exchangerate-dev Latest API
  slug: exchangerate-dev-latest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-latest-api-openapi.yml
- filename: exchangerate-dev-official-api-openapi.yml
  format: yaml
  label: exchangerate-dev Official API
  slug: exchangerate-dev-official-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-official-api-openapi.yml
- filename: exchangerate-dev-range-api-openapi.yml
  format: yaml
  label: exchangerate-dev Range API
  slug: exchangerate-dev-range-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-range-api-openapi.yml
- filename: exchangerate-dev-rate-api-openapi.yml
  format: yaml
  label: exchangerate-dev Rate API
  slug: exchangerate-dev-rate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-rate-api-openapi.yml
- filename: exchangerate-dev-status-api-openapi.yml
  format: yaml
  label: exchangerate-dev Status API
  slug: exchangerate-dev-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-status-api-openapi.yml
- filename: exchangerate-dev-webhooks-api-openapi.yml
  format: yaml
  label: exchangerate-dev Webhooks API
  slug: exchangerate-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-webhooks-api-openapi.yml
- filename: exchangerate-dev-time-series-api-openapi.yml
  format: yaml
  label: exchangerate-dev Time Series API
  slug: exchangerate-dev-time-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exchangerate-dev/openapi/exchangerate-dev-time-series-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: exchangerate.dev
  spf: true
hosts:
- cert_expires: Jan 20 18:06:14 2027 GMT
  host: exchangerate.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Exchangerate Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for exchangerate-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: exchangerate-dev
provider_slug: exchangerate-dev
slug: exchangerate-dev-domain-security
source_filename: exchangerate-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: exchangerate.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 18:06:14 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: exchangerate.dev\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/exchangerate-dev/security/exchangerate-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Finance
- Currency
- ExchangeRates
- API
---
