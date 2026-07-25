---
api_specs:
- filename: recharge-payments-addresses-api-openapi.yml
  format: yaml
  label: Recharge Addresses API
  slug: recharge-payments-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recharge-payments/refs/heads/main/openapi/recharge-payments-addresses-api-openapi.yml
- filename: recharge-payments-charges-api-openapi.yml
  format: yaml
  label: Recharge Charges API
  slug: recharge-payments-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recharge-payments/refs/heads/main/openapi/recharge-payments-charges-api-openapi.yml
- filename: recharge-payments-customers-api-openapi.yml
  format: yaml
  label: Recharge Customers API
  slug: recharge-payments-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recharge-payments/refs/heads/main/openapi/recharge-payments-customers-api-openapi.yml
- filename: recharge-payments-discounts-api-openapi.yml
  format: yaml
  label: Recharge Discounts API
  slug: recharge-payments-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recharge-payments/refs/heads/main/openapi/recharge-payments-discounts-api-openapi.yml
- filename: recharge-payments-onetimes-api-openapi.yml
  format: yaml
  label: Recharge Onetimes API
  slug: recharge-payments-onetimes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recharge-payments/refs/heads/main/openapi/recharge-payments-onetimes-api-openapi.yml
- filename: recharge-payments-orders-api-openapi.yml
  format: yaml
  label: Recharge Orders API
  slug: recharge-payments-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recharge-payments/refs/heads/main/openapi/recharge-payments-orders-api-openapi.yml
- filename: recharge-payments-payment-methods-api-openapi.yml
  format: yaml
  label: Recharge Payment Methods API
  slug: recharge-payments-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recharge-payments/refs/heads/main/openapi/recharge-payments-payment-methods-api-openapi.yml
- filename: recharge-payments-products-api-openapi.yml
  format: yaml
  label: Recharge Products API
  slug: recharge-payments-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recharge-payments/refs/heads/main/openapi/recharge-payments-products-api-openapi.yml
- filename: recharge-payments-subscriptions-api-openapi.yml
  format: yaml
  label: Recharge Subscriptions API
  slug: recharge-payments-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recharge-payments/refs/heads/main/openapi/recharge-payments-subscriptions-api-openapi.yml
- filename: recharge-payments-webhooks-api-openapi.yml
  format: yaml
  label: Recharge Webhooks API
  slug: recharge-payments-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recharge-payments/refs/heads/main/openapi/recharge-payments-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getrecharge.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rechargepayments.com
  spf: true
hosts:
- cert_expires: Aug 19 09:25:42 2026 GMT
  host: getrecharge.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 02:41:03 2026 GMT
  host: developer.rechargepayments.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 21:50:06 2026 GMT
  host: api.rechargeapps.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Recharge Payments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Recharge, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Recharge
provider_slug: recharge-payments
slug: recharge-payments-domain-security
source_filename: recharge-payments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getrecharge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 09:25:42 2026 GMT\n  hsts: false\n- host: developer.rechargepayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 02:41:03 2026 GMT\n  hsts: false\n- host: api.rechargeapps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 21:50:06 2026 GMT\n  hsts: null\ndomains:\n- domain: getrecharge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: rechargepayments.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recharge-payments/refs/heads/main/security/recharge-payments-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Subscriptions
- Recurring Billing
- E-commerce
- Payments
- Shopify
- Retention
---
