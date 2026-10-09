---
api_specs:
- filename: xrpay-connected-account-api-openapi.yml
  format: yaml
  label: XRPay Connected account API
  slug: xrpay-connected-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xrpay/refs/heads/main/openapi/xrpay-connected-account-api-openapi.yml
- filename: xrpay-payment-intents-api-openapi.yml
  format: yaml
  label: XRPay Payment intents API
  slug: xrpay-payment-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xrpay/refs/heads/main/openapi/xrpay-payment-intents-api-openapi.yml
- filename: xrpay-payouts-api-openapi.yml
  format: yaml
  label: XRPay Payouts API
  slug: xrpay-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xrpay/refs/heads/main/openapi/xrpay-payouts-api-openapi.yml
- filename: xrpay-payroll-api-openapi.yml
  format: yaml
  label: XRPay Payroll API
  slug: xrpay-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xrpay/refs/heads/main/openapi/xrpay-payroll-api-openapi.yml
- filename: xrpay-refunds-api-openapi.yml
  format: yaml
  label: XRPay Refunds API
  slug: xrpay-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xrpay/refs/heads/main/openapi/xrpay-refunds-api-openapi.yml
- filename: xrpay-sandbox-api-openapi.yml
  format: yaml
  label: XRPay Sandbox API
  slug: xrpay-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xrpay/refs/heads/main/openapi/xrpay-sandbox-api-openapi.yml
- filename: xrpay-webhooks-api-openapi.yml
  format: yaml
  label: XRPay Webhooks API
  slug: xrpay-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xrpay/refs/heads/main/openapi/xrpay-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: xrpay.it
  spf: false
hosts:
- cert_expires: Dec 10 19:12:48 2026 GMT
  host: www.xrpay.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Xrpay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for XRPay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: XRPay
provider_slug: xrpay
slug: xrpay-domain-security
source_filename: xrpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xrpay.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 19:12:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: xrpay.it\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xrpay/refs/heads/main/security/xrpay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Merchant Payments
- Refunds
- Webhooks
- Fintech
---
