---
api_specs:
- filename: asterpay-io-ai-api-openapi.yml
  format: yaml
  label: AsterPay AI API
  slug: asterpay-io-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-ai-api-openapi.yml
- filename: asterpay-io-crypto-api-openapi.yml
  format: yaml
  label: AsterPay Crypto API
  slug: asterpay-io-crypto-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-crypto-api-openapi.yml
- filename: asterpay-io-data-api-openapi.yml
  format: yaml
  label: AsterPay Data API
  slug: asterpay-io-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-data-api-openapi.yml
- filename: asterpay-io-discovery-api-openapi.yml
  format: yaml
  label: AsterPay Discovery API
  slug: asterpay-io-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-discovery-api-openapi.yml
- filename: asterpay-io-market-api-openapi.yml
  format: yaml
  label: AsterPay Market API
  slug: asterpay-io-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-market-api-openapi.yml
- filename: asterpay-io-sessions-api-openapi.yml
  format: yaml
  label: AsterPay Sessions API
  slug: asterpay-io-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-sessions-api-openapi.yml
- filename: asterpay-io-settlement-api-openapi.yml
  format: yaml
  label: AsterPay Settlement API
  slug: asterpay-io-settlement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-settlement-api-openapi.yml
- filename: asterpay-io-trust-api-openapi.yml
  format: yaml
  label: AsterPay Trust API
  slug: asterpay-io-trust-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-trust-api-openapi.yml
- filename: asterpay-io-utility-api-openapi.yml
  format: yaml
  label: AsterPay Utility API
  slug: asterpay-io-utility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-utility-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: asterpay.io
  spf: true
hosts:
- cert_expires: Dec 15 21:49:55 2026 GMT
  host: asterpay.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Asterpay Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AsterPay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: AsterPay
provider_slug: asterpay-io
slug: asterpay-io-domain-security
source_filename: asterpay-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asterpay.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 21:49:55 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: asterpay.io\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/asterpay-io/security/asterpay-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payments
- Fintech
- Artificial Intelligence
- EUR
- Settlement
---
