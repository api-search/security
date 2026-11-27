---
api_specs:
- filename: bitoasis-market-data-api-openapi.yml
  format: yaml
  label: BitOasis Market Data API
  slug: bitoasis-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitoasis/openapi/bitoasis-market-data-api-openapi.yml
- filename: bitoasis-accounts-api-openapi.yml
  format: yaml
  label: BitOasis Accounts API
  slug: bitoasis-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitoasis/openapi/bitoasis-accounts-api-openapi.yml
- filename: bitoasis-banks-api-openapi.yml
  format: yaml
  label: BitOasis Banks API
  slug: bitoasis-banks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitoasis/openapi/bitoasis-banks-api-openapi.yml
- filename: bitoasis-deposit-api-openapi.yml
  format: yaml
  label: BitOasis Deposit API
  slug: bitoasis-deposit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitoasis/openapi/bitoasis-deposit-api-openapi.yml
- filename: bitoasis-error-responses-api-openapi.yml
  format: yaml
  label: BitOasis Error responses API
  slug: bitoasis-error-responses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitoasis/openapi/bitoasis-error-responses-api-openapi.yml
- filename: bitoasis-order-api-openapi.yml
  format: yaml
  label: BitOasis Order API
  slug: bitoasis-order-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitoasis/openapi/bitoasis-order-api-openapi.yml
- filename: bitoasis-withdrawal-api-openapi.yml
  format: yaml
  label: BitOasis Withdrawal API
  slug: bitoasis-withdrawal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitoasis/openapi/bitoasis-withdrawal-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bitoasis.net
  spf: true
hosts:
- cert_expires: Oct  2 12:27:29 2026 GMT
  host: bitoasis.net
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 14:16:21 2026 GMT
  host: api.bitoasis.net
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: BitOasis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BitOasis, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BitOasis
provider_slug: bitoasis
slug: bitoasis-domain-security
source_filename: bitoasis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitoasis.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:27:29 2026 GMT\n  hsts: null\n- host: api.bitoasis.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 14:16:21 2026 GMT\n  hsts: null\ndomains:\n- domain: bitoasis.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/bitoasis/security/bitoasis-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Digital Assets
- Bitcoin
- MENA
- Fintech
- MCP
---
