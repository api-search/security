---
api_specs:
- filename: paystone-balance-portal-api-openapi.yml
  format: yaml
  label: Paystone Balance Portal API
  slug: paystone-balance-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-balance-portal-api-openapi.yml
- filename: paystone-client-management-api-openapi.yml
  format: yaml
  label: Paystone Client Management API
  slug: paystone-client-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-client-management-api-openapi.yml
- filename: paystone-contact-api-openapi.yml
  format: yaml
  label: Paystone Contact API
  slug: paystone-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-contact-api-openapi.yml
- filename: paystone-gift-account-type-api-openapi.yml
  format: yaml
  label: Paystone Gift Account Type API
  slug: paystone-gift-account-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-gift-account-type-api-openapi.yml
- filename: paystone-item-api-openapi.yml
  format: yaml
  label: Paystone Item API
  slug: paystone-item-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-item-api-openapi.yml
- filename: paystone-loyalty-account-type-api-openapi.yml
  format: yaml
  label: Paystone Loyalty Account Type API
  slug: paystone-loyalty-account-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-loyalty-account-type-api-openapi.yml
- filename: paystone-loyalty-transaction-api-openapi.yml
  format: yaml
  label: Paystone Loyalty Transaction API
  slug: paystone-loyalty-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-loyalty-transaction-api-openapi.yml
- filename: paystone-member-portal-api-openapi.yml
  format: yaml
  label: Paystone Member Portal API
  slug: paystone-member-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-member-portal-api-openapi.yml
- filename: paystone-merchant-management-api-openapi.yml
  format: yaml
  label: Paystone Merchant Management API
  slug: paystone-merchant-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-merchant-management-api-openapi.yml
- filename: paystone-prepaid-transaction-api-openapi.yml
  format: yaml
  label: Paystone Prepaid Transaction API
  slug: paystone-prepaid-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-prepaid-transaction-api-openapi.yml
- filename: paystone-promo-account-type-api-openapi.yml
  format: yaml
  label: Paystone Promo Account Type API
  slug: paystone-promo-account-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-promo-account-type-api-openapi.yml
- filename: paystone-reward-api-openapi.yml
  format: yaml
  label: Paystone Reward API
  slug: paystone-reward-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-reward-api-openapi.yml
- filename: paystone-user-management-api-openapi.yml
  format: yaml
  label: Paystone User Management API
  slug: paystone-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-user-management-api-openapi.yml
- filename: paystone-webhook-management-api-openapi.yml
  format: yaml
  label: Paystone Webhook Management API
  slug: paystone-webhook-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-webhook-management-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: paystone.com
  spf: true
hosts:
- cert_expires: Sep 26 17:32:29 2026 GMT
  host: www.paystone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 23:59:59 2026 GMT
  host: api.paystone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paystone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paystone, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Paystone
provider_slug: paystone
slug: paystone-domain-security
source_filename: paystone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paystone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 17:32:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.paystone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: paystone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/security/paystone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Canada
- Payment Processing
- Acquiring
- Gift Cards
- Loyalty
- Subscription
- Billing
- Merchant Services
---
