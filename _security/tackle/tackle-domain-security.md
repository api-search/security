---
api_specs:
- filename: tackle-api-openapi.json
  format: json
  label: Tackle API
  slug: tackle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/openapi/tackle-api-openapi.json
- filename: tackle-cosell-openapi.json
  format: json
  label: Tackle Co-Sell for AWS Partner Central
  slug: tackle-co-sell-for-aws-partner-central
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/openapi/tackle-cosell-openapi.json
- filename: tackle-marketplace-openapi.json
  format: json
  label: Tackle Offers (AWS Marketplace)
  slug: tackle-offers-aws-marketplace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/openapi/tackle-marketplace-openapi.json
- filename: tackle-offers-openapi.json
  format: json
  label: Tackle Offers (Microsoft Marketplace)
  slug: tackle-offers-microsoft-marketplace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/openapi/tackle-offers-openapi.json
- filename: tackle-contracts-openapi.json
  format: json
  label: Tackle Public Contracts API
  slug: tackle-public-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/openapi/tackle-contracts-openapi.json
- filename: tackle-prospect-openapi.json
  format: json
  label: Tackle Prospect API
  slug: tackle-prospect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/openapi/tackle-prospect-openapi.json
- filename: tackle-scim-openapi.json
  format: json
  label: Tackle SCIM API
  slug: tackle-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/openapi/tackle-scim-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tackle.io
  spf: true
hosts:
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: api.tackle.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: contracts.tackle.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 25 23:59:59 2027 GMT
  host: aws.cosell.tackle.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tackle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tackle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tackle
provider_slug: tackle
slug: tackle-domain-security
source_filename: tackle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.tackle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: contracts.tackle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: null\n- host: aws.cosell.tackle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: tackle.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/security/tackle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud Marketplace
- Cloud GTM
- Go-To-Market
- Private Offers
- Co-Sell
- Metering
- SCIM
- AWS Marketplace
- Azure Marketplace
---
