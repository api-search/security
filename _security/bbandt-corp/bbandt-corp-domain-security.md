---
api_specs:
- filename: bbandt-corp-commercial-accounts-openapi.yml
  format: yaml
  label: Truist Commercial Accounts
  slug: commercial-accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-commercial-accounts-openapi.yml
- filename: bbandt-corp-commercial-account-balance-openapi.yml
  format: yaml
  label: Truist Commercial Account Balance
  slug: commercial-account-balance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-commercial-account-balance-openapi.yml
- filename: bbandt-corp-commercial-account-transactions-openapi.yml
  format: yaml
  label: Truist Commercial Account Transactions
  slug: commercial-account-transactions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-commercial-account-transactions-openapi.yml
- filename: bbandt-corp-retail-accounts-openapi.yml
  format: yaml
  label: Truist Personal and Small Business Accounts
  slug: personal-small-business-accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-retail-accounts-openapi.yml
- filename: bbandt-corp-retail-locator-openapi.yml
  format: yaml
  label: Truist Branch/ATM Locator
  slug: branch-atm-locator
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-retail-locator-openapi.yml
- filename: bbandt-corp-retail-accounts-transaction-openapi.yml
  format: yaml
  label: Truist Personal and Small Business Transactions
  slug: personal-small-business-transactions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-retail-accounts-transaction-openapi.yml
- filename: bbandt-corp-retail-customers-openapi.yml
  format: yaml
  label: Truist Personal and Small Business Client Contact
  slug: personal-and-small-business-client-contact
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-retail-customers-openapi.yml
- filename: bbandt-corp-retail-auth-oauth-openapi.yml
  format: yaml
  label: Truist Retail Oauth Authentication
  slug: retail-oauth-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-retail-auth-oauth-openapi.yml
- filename: bbandt-corp-retail-consents-openapi.yml
  format: yaml
  label: Truist User Consent
  slug: user-consent
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-retail-consents-openapi.yml
- filename: bbandt-corp-retail-register-recipient-openapi.yml
  format: yaml
  label: Truist Retail Dynamic Client Registration
  slug: retail-dynamic-client-registration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-retail-register-recipient-openapi.yml
- filename: bbandt-corp-retail-payment-networks-openapi.yml
  format: yaml
  label: Truist Personal and Small Business Account Payment Networks
  slug: personal-and-small-business-account-payment-networks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-retail-payment-networks-openapi.yml
- filename: bbandt-corp-retail-accounts-contact-openapi.yml
  format: yaml
  label: Truist Account Address
  slug: account-address
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-retail-accounts-contact-openapi.yml
- filename: bbandt-corp-commercial-credit-transfers-oas-v2-openapi.yml
  format: yaml
  label: Truist Credit Transfers
  slug: credit-transfers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-commercial-credit-transfers-oas-v2-openapi.yml
- filename: bbandt-corp-retail-event-notifications-openapi.yml
  format: yaml
  label: Truist Personal and Small Business Event Notifications
  slug: personal-and-small-business-event-notifications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-retail-event-notifications-openapi.yml
- filename: bbandt-corp-retail-event-subscriptions-openapi.yml
  format: yaml
  label: Truist Personal and Small Business Event Subscriptions
  slug: personal-and-small-business-event-subscriptions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-retail-event-subscriptions-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 contactemail "ccs_certificate_services@truist.com"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: truist.com
  spf: true
hosts:
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: developer.truist.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: www.truist.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: api.truist.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Bbandt Corp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BB&T Corp (Truist), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BB&T Corp (Truist)
provider_slug: bbandt-corp
slug: bbandt-corp-domain-security
source_filename: bbandt-corp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.truist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: null\n- host: www.truist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.truist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: truist.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 contactemail \"ccs_certificate_services@truist.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/security/bbandt-corp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Financial-Services
- Open Banking
- Truist
- BB&T
- Fortune 500
---
