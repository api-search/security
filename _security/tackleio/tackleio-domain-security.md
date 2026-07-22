---
api_specs:
- filename: tackleio-platform-openapi.json
  format: json
  label: Tackle Platform API
  slug: tackle-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-platform-openapi.json
- filename: tackleio-prospect-openapi.json
  format: json
  label: Tackle Prospect API
  slug: tackle-prospect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-prospect-openapi.json
- filename: tackleio-cosell-aws-openapi.json
  format: json
  label: Tackle Co-Sell for AWS Partner Central
  slug: tackle-co-sell-for-aws-partner-central
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-cosell-aws-openapi.json
- filename: tackleio-cosell-gcp-openapi.json
  format: json
  label: Tackle Co-Sell for Google Cloud
  slug: tackle-co-sell-for-google-cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-cosell-gcp-openapi.json
- filename: tackleio-cosell-msft-openapi.json
  format: json
  label: Tackle Co-Sell for Microsoft Partner Center
  slug: tackle-co-sell-for-microsoft-partner-center
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-cosell-msft-openapi.json
- filename: tackleio-offers-aws-openapi.json
  format: json
  label: Tackle Offers for AWS Marketplace
  slug: tackle-offers-for-aws-marketplace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-offers-aws-openapi.json
- filename: tackleio-offers-msft-openapi.json
  format: json
  label: Tackle Offers for Microsoft
  slug: tackle-offers-for-microsoft
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-offers-msft-openapi.json
- filename: tackleio-contracts-openapi.json
  format: json
  label: Tackle Public Contracts API
  slug: tackle-public-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-contracts-openapi.json
- filename: tackleio-scim-openapi.json
  format: json
  label: Tackle SCIM API
  slug: tackle-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/openapi/tackleio-scim-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tackle.io
  spf: true
hosts:
- cert_expires: Sep 26 09:13:44 2026 GMT
  host: tackle.io
  hsts: true
  hsts_max_age: 63072000
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
name: Tackleio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tackle.io, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tackle.io
provider_slug: tackleio
slug: tackleio-domain-security
source_filename: tackleio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tackle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 09:13:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: contracts.tackle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: null\n- host: aws.cosell.tackle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: tackle.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tackleio/refs/heads/main/security/tackleio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud
- Cloud Marketplace
- Co-Sell
- AWS Marketplace
- Azure Marketplace
- Google Cloud Marketplace
- Private Offers
- Metering
- SCIM
- Webhooks
- B2B SaaS
---
