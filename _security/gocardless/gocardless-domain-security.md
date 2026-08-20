---
api_specs:
- filename: gocardless-billing-request-flows-api-openapi.yml
  format: yaml
  label: GoCardless billing_request_flows API
  slug: gocardless-billing-request-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-billing-request-flows-api-openapi.yml
- filename: gocardless-billing-requests-api-openapi.yml
  format: yaml
  label: GoCardless billing_requests API
  slug: gocardless-billing-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-billing-requests-api-openapi.yml
- filename: gocardless-blocks-api-openapi.yml
  format: yaml
  label: GoCardless blocks API
  slug: gocardless-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-blocks-api-openapi.yml
- filename: gocardless-creditor-bank-accounts-api-openapi.yml
  format: yaml
  label: GoCardless creditor_bank_accounts API
  slug: gocardless-creditor-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-creditor-bank-accounts-api-openapi.yml
- filename: gocardless-creditors-api-openapi.yml
  format: yaml
  label: GoCardless creditors API
  slug: gocardless-creditors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-creditors-api-openapi.yml
- filename: gocardless-customer-bank-accounts-api-openapi.yml
  format: yaml
  label: GoCardless customer_bank_accounts API
  slug: gocardless-customer-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-customer-bank-accounts-api-openapi.yml
- filename: gocardless-customers-api-openapi.yml
  format: yaml
  label: GoCardless customers API
  slug: gocardless-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-customers-api-openapi.yml
- filename: gocardless-events-api-openapi.yml
  format: yaml
  label: GoCardless events API
  slug: gocardless-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-events-api-openapi.yml
- filename: gocardless-instalment-schedules-api-openapi.yml
  format: yaml
  label: GoCardless instalment_schedules API
  slug: gocardless-instalment-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-instalment-schedules-api-openapi.yml
- filename: gocardless-institutions-api-openapi.yml
  format: yaml
  label: GoCardless institutions API
  slug: gocardless-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-institutions-api-openapi.yml
- filename: gocardless-mandates-api-openapi.yml
  format: yaml
  label: GoCardless mandates API
  slug: gocardless-mandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-mandates-api-openapi.yml
- filename: gocardless-payer-authorisations-api-openapi.yml
  format: yaml
  label: GoCardless payer_authorisations API
  slug: gocardless-payer-authorisations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-payer-authorisations-api-openapi.yml
- filename: gocardless-payments-api-openapi.yml
  format: yaml
  label: GoCardless payments API
  slug: gocardless-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-payments-api-openapi.yml
- filename: gocardless-payouts-api-openapi.yml
  format: yaml
  label: GoCardless payouts API
  slug: gocardless-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-payouts-api-openapi.yml
- filename: gocardless-refunds-api-openapi.yml
  format: yaml
  label: GoCardless refunds API
  slug: gocardless-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-refunds-api-openapi.yml
- filename: gocardless-subscriptions-api-openapi.yml
  format: yaml
  label: GoCardless subscriptions API
  slug: gocardless-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-subscriptions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:core-infrastructure-ext@gocardless.com"
  - 0 issue "actalis.it"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gocardless.com
  spf: true
hosts:
- cert_expires: Aug 27 02:05:31 2026 GMT
  host: gocardless.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 17:33:00 2026 GMT
  host: developer.gocardless.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 23:06:15 2026 GMT
  host: api.gocardless.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gocardless Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoCardless, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GoCardless
provider_slug: gocardless
slug: gocardless-domain-security
source_filename: gocardless-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gocardless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 02:05:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: developer.gocardless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 17:33:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: api.gocardless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:06:15 2026 GMT\n  hsts: null\ndomains:\n- domain: gocardless.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:core-infrastructure-ext@gocardless.com\"\n  - 0 issue \"actalis.it\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/security/gocardless-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Direct Debit
- Bank Debit
- Recurring Payments
- Subscription
- SEPA
- Bacs
- ACH
- Open Banking
- Fintech
---
