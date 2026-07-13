---
api_specs:
- filename: paystack-accept-payments-openapi.yml
  format: yaml
  label: Paystack Accept Payments API
  slug: paystack-accept-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-accept-payments-openapi.yml
- filename: paystack-subscriptions-openapi.yml
  format: yaml
  label: Paystack Subscriptions API
  slug: paystack-subscriptions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-subscriptions-openapi.yml
- filename: paystack-customers-openapi.yml
  format: yaml
  label: Paystack Customers API
  slug: paystack-customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-customers-openapi.yml
- filename: paystack-transfers-openapi.yml
  format: yaml
  label: Paystack Transfers API
  slug: paystack-transfers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-transfers-openapi.yml
- filename: paystack-splits-subaccounts-openapi.yml
  format: yaml
  label: Paystack Splits and Subaccounts API
  slug: paystack-splits-subaccounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-splits-subaccounts-openapi.yml
- filename: paystack-dedicated-virtual-accounts-openapi.yml
  format: yaml
  label: Paystack Dedicated Virtual Accounts API
  slug: paystack-dedicated-virtual-accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-dedicated-virtual-accounts-openapi.yml
- filename: paystack-products-pages-openapi.yml
  format: yaml
  label: Paystack Products and Payment Pages API
  slug: paystack-products-pages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-products-pages-openapi.yml
- filename: paystack-payment-requests-openapi.yml
  format: yaml
  label: Paystack Payment Requests API
  slug: paystack-payment-requests
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-payment-requests-openapi.yml
- filename: paystack-refunds-disputes-openapi.yml
  format: yaml
  label: Paystack Refunds and Disputes API
  slug: paystack-refunds-disputes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-refunds-disputes-openapi.yml
- filename: paystack-settlements-openapi.yml
  format: yaml
  label: Paystack Settlements API
  slug: paystack-settlements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-settlements-openapi.yml
- filename: paystack-verification-openapi.yml
  format: yaml
  label: Paystack Verification API
  slug: paystack-verification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-verification-openapi.yml
- filename: paystack-balance-openapi.yml
  format: yaml
  label: Paystack Balance API
  slug: paystack-balance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-balance-openapi.yml
- filename: paystack-integration-openapi.yml
  format: yaml
  label: Paystack Integration Settings API
  slug: paystack-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-integration-openapi.yml
- filename: paystack-webhooks-asyncapi.yml
  format: yaml
  label: Paystack Webhooks
  slug: paystack-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/asyncapi/paystack-webhooks-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: paystack.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: paystack.co
  spf: true
hosts:
- cert_expires: Oct  4 16:51:31 2026 GMT
  host: paystack.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 06:32:05 2026 GMT
  host: api.paystack.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paystack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paystack, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Paystack
provider_slug: paystack
slug: paystack-domain-security
source_filename: paystack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paystack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 16:51:31 2026 GMT\n  hsts: null\n- host: api.paystack.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 06:32:05 2026 GMT\n  hsts: null\ndomains:\n- domain: paystack.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: paystack.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/security/paystack-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Africa
- Fintech
- Recurring Billing
- Marketplaces
- Payouts
- Mobile Money
- Stripe
---
