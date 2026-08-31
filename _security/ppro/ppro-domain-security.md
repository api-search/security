---
api_specs:
- filename: ppro-authorization-endpoints-api-openapi.yml
  format: yaml
  label: PPRO Authorization Endpoints API
  slug: ppro-authorization-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-authorization-endpoints-api-openapi.yml
- filename: ppro-capture-endpoints-api-openapi.yml
  format: yaml
  label: PPRO Capture Endpoints API
  slug: ppro-capture-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-capture-endpoints-api-openapi.yml
- filename: ppro-dispute-reports-api-openapi.yml
  format: yaml
  label: PPRO Dispute Reports API
  slug: ppro-dispute-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-dispute-reports-api-openapi.yml
- filename: ppro-disputes-api-openapi.yml
  format: yaml
  label: PPRO Disputes API
  slug: ppro-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-disputes-api-openapi.yml
- filename: ppro-enrollment-endpoints-api-openapi.yml
  format: yaml
  label: PPRO Enrollment Endpoints API
  slug: ppro-enrollment-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-enrollment-endpoints-api-openapi.yml
- filename: ppro-internal-api-openapi.yml
  format: yaml
  label: PPRO Internal API
  slug: ppro-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-internal-api-openapi.yml
- filename: ppro-merchants-api-openapi.yml
  format: yaml
  label: PPRO Merchants API
  slug: ppro-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-merchants-api-openapi.yml
- filename: ppro-payment-agreement-revocations-api-openapi.yml
  format: yaml
  label: PPRO Payment Agreement Revocations API
  slug: ppro-payment-agreement-revocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-payment-agreement-revocations-api-openapi.yml
- filename: ppro-payment-agreements-api-openapi.yml
  format: yaml
  label: PPRO Payment Agreements API
  slug: ppro-payment-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-payment-agreements-api-openapi.yml
- filename: ppro-payment-charge-controller-api-openapi.yml
  format: yaml
  label: PPRO Payment Charge Controller API
  slug: ppro-payment-charge-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-payment-charge-controller-api-openapi.yml
- filename: ppro-payment-charges-api-openapi.yml
  format: yaml
  label: PPRO Payment Charges API
  slug: ppro-payment-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-payment-charges-api-openapi.yml
- filename: ppro-payment-instruments-api-openapi.yml
  format: yaml
  label: PPRO Payment Instruments API
  slug: ppro-payment-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-payment-instruments-api-openapi.yml
- filename: ppro-payment-sessions-api-openapi.yml
  format: yaml
  label: PPRO Payment Sessions API
  slug: ppro-payment-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-payment-sessions-api-openapi.yml
- filename: ppro-people-api-openapi.yml
  format: yaml
  label: PPRO People API
  slug: ppro-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-people-api-openapi.yml
- filename: ppro-platforms-api-openapi.yml
  format: yaml
  label: PPRO Platforms API
  slug: ppro-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-platforms-api-openapi.yml
- filename: ppro-psps-api-openapi.yml
  format: yaml
  label: PPRO PS Ps API
  slug: ppro-psps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-psps-api-openapi.yml
- filename: ppro-refund-endpoints-api-openapi.yml
  format: yaml
  label: PPRO Refund Endpoints API
  slug: ppro-refund-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-refund-endpoints-api-openapi.yml
- filename: ppro-void-endpoints-api-openapi.yml
  format: yaml
  label: PPRO Void Endpoints API
  slug: ppro-void-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-void-endpoints-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: ppro.com
  spf: true
hosts:
- cert_expires: Nov 23 11:43:01 2026 GMT
  host: www.ppro.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 12:49:55 2026 GMT
  host: developerhub.ppro.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: api.eu.ppro.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ppro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PPRO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: PPRO
provider_slug: ppro
slug: ppro-domain-security
source_filename: ppro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ppro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 11:43:01 2026 GMT\n  hsts: null\n- host: developerhub.ppro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 12:49:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.eu.ppro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ppro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/security/ppro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Local Payment Methods
- Financial-Services
- Fintech
- Acquiring
- Checkout
- E-Commerce
- Digital Wallet
- Recurring Payments
- Disputes
- Chargebacks
- Company
---
