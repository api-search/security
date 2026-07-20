---
api_specs:
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Authorization API
  slug: mpesa-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Express (STK Push) API
  slug: mpesa-express-stk-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Customer To Business (C2B) API
  slug: mpesa-c2b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Business To Customer (B2C) API
  slug: mpesa-b2c-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Business To Business (B2B) API
  slug: mpesa-b2b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa B2B Express Checkout (USSD Push) API
  slug: mpesa-b2b-express-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Transaction Status API
  slug: mpesa-transaction-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Account Balance API
  slug: mpesa-account-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Reversal API
  slug: mpesa-reversal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Dynamic QR Code API
  slug: mpesa-dynamic-qr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Tax Remittance API
  slug: mpesa-tax-remittance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Bill Manager API
  slug: mpesa-bill-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Ratiba (Standing Order) API
  slug: mpesa-ratiba-standing-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
description: ''
domains:
- dmarc: true
  dmarc_policy: reject
  dmarc_subdomain_policy: reject
  domain: safaricom.co.ke
  spf: true
  spf_policy: ~all
hosts:
- cert_expires: Nov 18 23:59:59 2026 GMT
  cert_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1
  host: developer.safaricom.co.ke
  hsts: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
- cert_expires: Oct  6 23:59:59 2026 GMT
  cert_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1
  host: api.safaricom.co.ke
  hsts: null
  http_note: Production API gateway; root returns 404, product paths live under /mpesa/*, /oauth/*.
  http_status: 404
  https: true
- cert_expires: Sep  8 23:59:59 2026 GMT
  cert_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1
  host: sandbox.safaricom.co.ke
  hsts: true
  hsts_max_age: 31536000
  http_note: Sandbox API gateway; root returns 404, product paths live under /mpesa/*, /oauth/*.
  http_status: 404
  https: true
kind: domain-security
layout: security
method: probed
name: Mpesa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for M-Pesa (Safaricom Daraja), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS; 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: M-Pesa (Safaricom Daraja)
provider_slug: mpesa
slug: mpesa-domain-security
source_filename: mpesa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.safaricom.co.ke\n  https: true\n  http_status: 200\n  cert_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.safaricom.co.ke\n  https: true\n  http_status: 404\n  http_note: Production API gateway; root returns 404, product paths live under /mpesa/*, /oauth/*.\n  cert_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: null\n- host: sandbox.safaricom.co.ke\n  https: true\n  http_status: 404\n  http_note: Sandbox API gateway; root returns 404, product paths live under /mpesa/*, /oauth/*.\n  cert_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1\n  cert_expires: Sep  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: safaricom.co.ke\n  spf: true\n  spf_policy: ~all\n  dmarc:\
  \ true\n  dmarc_policy: reject\n  dmarc_subdomain_policy: reject\nnotes: >-\n  All Daraja hosts serve HTTPS with DigiCert-issued certificates. Parent domain\n  safaricom.co.ke publishes SPF (softfail) and a strict DMARC reject policy. Beyond\n  transport security, Daraja funds-movement operations require an application-layer\n  SecurityCredential (initiator password RSA-encrypted with Safaricom's M-Pesa public\n  X.509 certificate).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/security/mpesa-domain-security.yml
summary_line: HSTS · DMARC
tags:
- Mobile Money
- Payments
- Fintech
- Kenya
- Africa
- M-Pesa
---
