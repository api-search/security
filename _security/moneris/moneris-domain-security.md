---
api_specs:
- filename: moneris-3d-secure-api-openapi.yml
  format: yaml
  label: Moneris 3D Secure API
  slug: moneris-3d-secure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-3d-secure-api-openapi.yml
- filename: moneris-customers-api-openapi.yml
  format: yaml
  label: Moneris Customers API
  slug: moneris-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-customers-api-openapi.yml
- filename: moneris-disputes-api-openapi.yml
  format: yaml
  label: Moneris Disputes API
  slug: moneris-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-disputes-api-openapi.yml
- filename: moneris-installments-api-openapi.yml
  format: yaml
  label: Moneris Installments API
  slug: moneris-installments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-installments-api-openapi.yml
- filename: moneris-kount-api-openapi.yml
  format: yaml
  label: Moneris Kount API
  slug: moneris-kount-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-kount-api-openapi.yml
- filename: moneris-merchant-onboarding-api-openapi.yml
  format: yaml
  label: Moneris Merchant Onboarding API
  slug: moneris-merchant-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-merchant-onboarding-api-openapi.yml
- filename: moneris-multi-currency-pricing-rate-lookup-api-openapi.yml
  format: yaml
  label: Moneris Multi-Currency Pricing Rate Lookup API
  slug: moneris-multi-currency-pricing-rate-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-multi-currency-pricing-rate-lookup-api-openapi.yml
- filename: moneris-payment-methods-api-openapi.yml
  format: yaml
  label: Moneris Payment Methods API
  slug: moneris-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-payment-methods-api-openapi.yml
- filename: moneris-payments-api-openapi.yml
  format: yaml
  label: Moneris Payments API
  slug: moneris-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-payments-api-openapi.yml
- filename: moneris-products-api-openapi.yml
  format: yaml
  label: Moneris Products API
  slug: moneris-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-products-api-openapi.yml
- filename: moneris-refunds-api-openapi.yml
  format: yaml
  label: Moneris Refunds API
  slug: moneris-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-refunds-api-openapi.yml
- filename: moneris-subscriptions-api-openapi.yml
  format: yaml
  label: Moneris Subscriptions API
  slug: moneris-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-subscriptions-api-openapi.yml
- filename: moneris-surcharge-lookup-api-openapi.yml
  format: yaml
  label: Moneris Surcharge Lookup API
  slug: moneris-surcharge-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-surcharge-lookup-api-openapi.yml
- filename: moneris-terminal-service-orders-api-openapi.yml
  format: yaml
  label: Moneris Terminal & Service Orders API
  slug: moneris-terminal-service-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-terminal-service-orders-api-openapi.yml
- filename: moneris-validations-api-openapi.yml
  format: yaml
  label: Moneris Validations API
  slug: moneris-validations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-validations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: moneris.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: moneris.io
  spf: true
hosts:
- cert_expires: Sep 19 20:43:54 2026 GMT
  host: www.moneris.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 02:38:17 2026 GMT
  host: developer.moneris.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: api.moneris.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moneris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moneris, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Moneris
provider_slug: moneris
slug: moneris-domain-security
source_filename: moneris-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moneris.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 20:43:54 2026 GMT\n  hsts: false\n- host: developer.moneris.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 02:38:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.moneris.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: moneris.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: moneris.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/security/moneris-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Payments
- Payment Processing
- Card Payments
- Merchant Services
- Acquiring
- Canada
- Fintech
- Infrastructure
---
