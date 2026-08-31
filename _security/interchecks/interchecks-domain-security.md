---
api_specs:
- filename: interchecks-accounts-api-openapi.yml
  format: yaml
  label: Interchecks Accounts API
  slug: interchecks-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-accounts-api-openapi.yml
- filename: interchecks-authentication-api-openapi.yml
  format: yaml
  label: Interchecks Authentication API
  slug: interchecks-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-authentication-api-openapi.yml
- filename: interchecks-oauth2-api-openapi.yml
  format: yaml
  label: Interchecks Oauth2 API
  slug: interchecks-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-oauth2-api-openapi.yml
- filename: interchecks-payers-api-openapi.yml
  format: yaml
  label: Interchecks Payers API
  slug: interchecks-payers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-payers-api-openapi.yml
- filename: interchecks-payload-api-openapi.yml
  format: yaml
  label: Interchecks Payload API
  slug: interchecks-payload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-payload-api-openapi.yml
- filename: interchecks-payment-accounts-bank-api-openapi.yml
  format: yaml
  label: Interchecks Payment Accounts - Bank API
  slug: interchecks-payment-accounts-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-payment-accounts-bank-api-openapi.yml
- filename: interchecks-payment-accounts-card-api-openapi.yml
  format: yaml
  label: Interchecks Payment Accounts - Card API
  slug: interchecks-payment-accounts-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-payment-accounts-card-api-openapi.yml
- filename: interchecks-payment-accounts-paypal-api-openapi.yml
  format: yaml
  label: Interchecks Payment Accounts - PayPal API
  slug: interchecks-payment-accounts-paypal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-payment-accounts-paypal-api-openapi.yml
- filename: interchecks-payments-api-openapi.yml
  format: yaml
  label: Interchecks Payments API
  slug: interchecks-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-payments-api-openapi.yml
- filename: interchecks-recipient-emails-api-openapi.yml
  format: yaml
  label: Interchecks Recipient Emails API
  slug: interchecks-recipient-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-recipient-emails-api-openapi.yml
- filename: interchecks-recipient-verification-api-openapi.yml
  format: yaml
  label: Interchecks Recipient Verification API
  slug: interchecks-recipient-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-recipient-verification-api-openapi.yml
- filename: interchecks-recipients-api-openapi.yml
  format: yaml
  label: Interchecks Recipients API
  slug: interchecks-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-recipients-api-openapi.yml
- filename: interchecks-reports-api-openapi.yml
  format: yaml
  label: Interchecks Reports API
  slug: interchecks-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-reports-api-openapi.yml
- filename: interchecks-test-harness-api-openapi.yml
  format: yaml
  label: Interchecks Test Harness API
  slug: interchecks-test-harness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-test-harness-api-openapi.yml
- filename: interchecks-transactions-api-openapi.yml
  format: yaml
  label: Interchecks Transactions API
  slug: interchecks-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-transactions-api-openapi.yml
- filename: interchecks-widgets-api-openapi.yml
  format: yaml
  label: Interchecks Widgets API
  slug: interchecks-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/openapi/interchecks-widgets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: interchecks.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: interchecks.io
  spf: false
hosts:
- cert_expires: Oct 30 18:14:29 2026 GMT
  host: home.interchecks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 12:12:04 2026 GMT
  host: docs-v2.interchecks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 16:36:08 2026 GMT
  host: prod.api.interchecks.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Interchecks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Interchecks, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Interchecks
provider_slug: interchecks
slug: interchecks-domain-security
source_filename: interchecks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: home.interchecks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 18:14:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs-v2.interchecks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 12:12:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: prod.api.interchecks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 16:36:08 2026 GMT\n  hsts: null\ndomains:\n- domain: interchecks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: interchecks.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interchecks/refs/heads/main/security/interchecks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payouts
- ACH
- Real-Time Payments
- Instant Payments
- Disbursements
- Cards
- Financial Services
- Fintech
- Webhooks
---
