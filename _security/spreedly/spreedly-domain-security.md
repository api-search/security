---
api_specs:
- filename: spreedly-api-v1.json
  format: json
  label: Spreedly Core Transactional API
  slug: spreedly-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreedly/refs/heads/main/openapi/spreedly-api-v1.json
- filename: spreedly-api-v1.json
  format: json
  label: Spreedly Payment Methods & Vault API
  slug: spreedly-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreedly/refs/heads/main/openapi/spreedly-api-v1.json
- filename: spreedly-api-v1.json
  format: json
  label: Spreedly Composer (Workflows) API
  slug: spreedly-composer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreedly/refs/heads/main/openapi/spreedly-api-v1.json
- filename: spreedly-api-v1.json
  format: json
  label: Spreedly Network Tokenization API
  slug: spreedly-network-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreedly/refs/heads/main/openapi/spreedly-api-v1.json
- filename: spreedly-api-v1.json
  format: json
  label: Spreedly Account Updater (Card Refresher) API
  slug: spreedly-account-updater-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreedly/refs/heads/main/openapi/spreedly-api-v1.json
- filename: spreedly-api-v1.json
  format: json
  label: Spreedly Receivers API
  slug: spreedly-receivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreedly/refs/heads/main/openapi/spreedly-api-v1.json
- filename: spreedly-api-v1.json
  format: json
  label: Spreedly 3-D Secure / SCA Authentication API
  slug: spreedly-sca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreedly/refs/heads/main/openapi/spreedly-api-v1.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: spreedly.com
  spf: true
hosts:
- cert_expires: Oct 14 17:05:28 2026 GMT
  host: www.spreedly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 05:10:35 2026 GMT
  host: developer.spreedly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 13:36:59 2026 GMT
  host: core.spreedly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spreedly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spreedly, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Spreedly
provider_slug: spreedly
slug: spreedly-domain-security
source_filename: spreedly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spreedly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 17:05:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.spreedly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 05:10:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: core.spreedly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 13:36:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: spreedly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spreedly/refs/heads/main/security/spreedly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- United States
- Payment Gateway
- Payment Orchestration
- Payment Processing
- Card Vault
- Tokenization
- Network Tokenization
- PCI Compliance
- Subscriptions
---
