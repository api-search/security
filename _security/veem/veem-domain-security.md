---
api_specs:
- filename: veem-attachment-controller-api-openapi.yml
  format: yaml
  label: Veem attachment-controller API
  slug: veem-attachment-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veem/refs/heads/main/openapi/veem-attachment-controller-api-openapi.yml
- filename: veem-bank-account-controller-api-openapi.yml
  format: yaml
  label: Veem bank-account-controller API
  slug: veem-bank-account-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veem/refs/heads/main/openapi/veem-bank-account-controller-api-openapi.yml
- filename: veem-beneficial-owner-information-controller-api-openapi.yml
  format: yaml
  label: Veem beneficial-owner-information-controller API
  slug: veem-beneficial-owner-information-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veem/refs/heads/main/openapi/veem-beneficial-owner-information-controller-api-openapi.yml
- filename: veem-claimless-payment-controller-api-openapi.yml
  format: yaml
  label: Veem claimless-payment-controller API
  slug: veem-claimless-payment-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veem/refs/heads/main/openapi/veem-claimless-payment-controller-api-openapi.yml
- filename: veem-contact-controller-api-openapi.yml
  format: yaml
  label: Veem contact-controller API
  slug: veem-contact-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veem/refs/heads/main/openapi/veem-contact-controller-api-openapi.yml
- filename: veem-crypto-wallet-controller-api-openapi.yml
  format: yaml
  label: Veem crypto-wallet-controller API
  slug: veem-crypto-wallet-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veem/refs/heads/main/openapi/veem-crypto-wallet-controller-api-openapi.yml
- filename: veem-customer-controller-api-openapi.yml
  format: yaml
  label: Veem customer-controller API
  slug: veem-customer-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veem/refs/heads/main/openapi/veem-customer-controller-api-openapi.yml
- filename: veem-exchange-rate-controller-api-openapi.yml
  format: yaml
  label: Veem exchange-rate-controller API
  slug: veem-exchange-rate-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veem/refs/heads/main/openapi/veem-exchange-rate-controller-api-openapi.yml
- filename: veem-invoice-controller-api-openapi.yml
  format: yaml
  label: Veem invoice-controller API
  slug: veem-invoice-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veem/refs/heads/main/openapi/veem-invoice-controller-api-openapi.yml
- filename: veem-meta-controller-api-openapi.yml
  format: yaml
  label: Veem meta-controller API
  slug: veem-meta-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veem/refs/heads/main/openapi/veem-meta-controller-api-openapi.yml
- filename: veem-open-account-controller-api-openapi.yml
  format: yaml
  label: Veem open-account-controller API
  slug: veem-open-account-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veem/refs/heads/main/openapi/veem-open-account-controller-api-openapi.yml
- filename: veem-payment-controller-api-openapi.yml
  format: yaml
  label: Veem payment-controller API
  slug: veem-payment-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veem/refs/heads/main/openapi/veem-payment-controller-api-openapi.yml
- filename: veem-wallet-controller-api-openapi.yml
  format: yaml
  label: Veem wallet-controller API
  slug: veem-wallet-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veem/refs/heads/main/openapi/veem-wallet-controller-api-openapi.yml
- filename: veem-webhook-controller-api-openapi.yml
  format: yaml
  label: Veem webhook-controller API
  slug: veem-webhook-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veem/refs/heads/main/openapi/veem-webhook-controller-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: veem.com
  spf: true
hosts:
- cert_expires: Oct 13 16:04:27 2026 GMT
  host: veem.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 05:08:33 2026 GMT
  host: sandbox-api.veem.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Veem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Veem, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Veem
provider_slug: veem
slug: veem-domain-security
source_filename: veem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: veem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 16:04:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox-api.veem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 05:08:33 2026 GMT\n  hsts: null\ndomains:\n- domain: veem.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veem/refs/heads/main/security/veem-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- B2B Payments
- Cross-Border Payments
- Invoicing
- Wallets
- Fintech
- Global Payments
---
