---
api_specs:
- filename: qualpay-account-updater-api-openapi.yml
  format: yaml
  label: Qualpay Account Updater API
  slug: qualpay-account-updater-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-account-updater-api-openapi.yml
- filename: qualpay-application-boarding-api-openapi.yml
  format: yaml
  label: Qualpay Application Boarding API
  slug: qualpay-application-boarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-application-boarding-api-openapi.yml
- filename: qualpay-checkout-api-openapi.yml
  format: yaml
  label: Qualpay Checkout API
  slug: qualpay-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-checkout-api-openapi.yml
- filename: qualpay-customer-vault-api-openapi.yml
  format: yaml
  label: Qualpay Customer Vault API
  slug: qualpay-customer-vault-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-customer-vault-api-openapi.yml
- filename: qualpay-disputes-v0-5-api-openapi.yml
  format: yaml
  label: Qualpay Disputes v0.5 API
  slug: qualpay-disputes-v0-5-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-disputes-v0-5-api-openapi.yml
- filename: qualpay-disputes-v1-0-api-openapi.yml
  format: yaml
  label: Qualpay Disputes v1.0 API
  slug: qualpay-disputes-v1-0-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-disputes-v1-0-api-openapi.yml
- filename: qualpay-embedded-fields-api-openapi.yml
  format: yaml
  label: Qualpay Embedded Fields API
  slug: qualpay-embedded-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-embedded-fields-api-openapi.yml
- filename: qualpay-integrator-api-openapi.yml
  format: yaml
  label: Qualpay Integrator API
  slug: qualpay-integrator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-integrator-api-openapi.yml
- filename: qualpay-invoicing-api-openapi.yml
  format: yaml
  label: Qualpay Invoicing API
  slug: qualpay-invoicing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-invoicing-api-openapi.yml
- filename: qualpay-payee-vault-api-openapi.yml
  format: yaml
  label: Qualpay Payee Vault API
  slug: qualpay-payee-vault-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-payee-vault-api-openapi.yml
- filename: qualpay-payment-gateway-api-openapi.yml
  format: yaml
  label: Qualpay Payment Gateway API
  slug: qualpay-payment-gateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-payment-gateway-api-openapi.yml
- filename: qualpay-recurring-billing-api-openapi.yml
  format: yaml
  label: Qualpay Recurring Billing API
  slug: qualpay-recurring-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-recurring-billing-api-openapi.yml
- filename: qualpay-reporting-api-openapi.yml
  format: yaml
  label: Qualpay Reporting API
  slug: qualpay-reporting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-reporting-api-openapi.yml
- filename: qualpay-token-api-openapi.yml
  format: yaml
  label: Qualpay Token API
  slug: qualpay-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-token-api-openapi.yml
- filename: qualpay-transaction-api-openapi.yml
  format: yaml
  label: Qualpay Transaction API
  slug: qualpay-transaction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-transaction-api-openapi.yml
- filename: qualpay-webhooks-api-openapi.yml
  format: yaml
  label: Qualpay Webhooks API
  slug: qualpay-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qualpay/openapi/qualpay-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "Digicert.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "entrust.net"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: qualpay.com
  spf: true
hosts:
- cert_expires: Dec 12 10:13:58 2026 GMT
  host: www.qualpay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Qualpay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qualpay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Qualpay
provider_slug: qualpay
slug: qualpay-domain-security
source_filename: qualpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qualpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 10:13:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: qualpay.com\n  dnssec: false\n  caa:\n  - 0 issue \"Digicert.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/qualpay/security/qualpay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Processing
- Merchant Services
- B2B Payments
- Reporting
- Tokenization
---
