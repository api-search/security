---
api_specs:
- filename: interswitch-web-checkout-api-openapi.yml
  format: yaml
  label: Interswitch Web Checkout API
  slug: interswitch-web-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-web-checkout-api-openapi.yml
- filename: interswitch-payment-gateway-api-openapi.yml
  format: yaml
  label: Interswitch Payment Gateway API
  slug: interswitch-payment-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-payment-gateway-api-openapi.yml
- filename: interswitch-transfers-api-openapi.yml
  format: yaml
  label: Interswitch Transfers API
  slug: interswitch-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-transfers-api-openapi.yml
- filename: interswitch-bills-payment-api-openapi.yml
  format: yaml
  label: Interswitch Bills Payment API
  slug: interswitch-bills-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-bills-payment-api-openapi.yml
- filename: interswitch-airtime-recharge-api-openapi.yml
  format: yaml
  label: Interswitch Airtime Recharge API
  slug: interswitch-airtime-recharge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-airtime-recharge-api-openapi.yml
- filename: interswitch-paycode-api-openapi.yml
  format: yaml
  label: Interswitch Paycode API
  slug: interswitch-paycode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-paycode-api-openapi.yml
- filename: interswitch-refunds-api-openapi.yml
  format: yaml
  label: Interswitch Refunds API
  slug: interswitch-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-refunds-api-openapi.yml
- filename: interswitch-recurring-payments-api-openapi.yml
  format: yaml
  label: Interswitch Recurring Payments API
  slug: interswitch-recurring-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-recurring-payments-api-openapi.yml
- filename: interswitch-card-360-api-openapi.yml
  format: yaml
  label: Interswitch Card 360 API
  slug: interswitch-card-360-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-card-360-api-openapi.yml
- filename: interswitch-lending-api-openapi.yml
  format: yaml
  label: Interswitch Lending API
  slug: interswitch-lending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-lending-api-openapi.yml
- filename: interswitch-customer-insights-api-openapi.yml
  format: yaml
  label: Interswitch Customer Insights API
  slug: interswitch-customer-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-customer-insights-api-openapi.yml
- filename: interswitch-transaction-search-api-openapi.yml
  format: yaml
  label: Interswitch Transaction Search API
  slug: interswitch-transaction-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-transaction-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: interswitchgroup.com
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: www.interswitchgroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 10:44:17 2026 GMT
  host: developer.interswitchgroup.com
  hsts: true
  hsts_max_age: 631138519
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 18:16:19 2026 GMT
  host: docs.interswitchgroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Interswitch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Interswitch, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Interswitch
provider_slug: interswitch
slug: interswitch-domain-security
source_filename: interswitch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.interswitchgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.interswitchgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 10:44:17 2026 GMT\n  hsts: true\n  hsts_max_age: 631138519\n- host: docs.interswitchgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 18:16:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: interswitchgroup.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/security/interswitch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payments
- Payment Infrastructure
- Card Network
- Verve
- Quickteller
- Webpay
- Bills Payment
- Transfers
- Lending
- Fintech
- Africa
- Nigeria
---
