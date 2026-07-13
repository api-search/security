---
api_specs:
- filename: myfatoorah-openapi.yml
  format: yaml
  label: MyFatoorah Payments API
  slug: myfatoorah-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-openapi.yml
- filename: myfatoorah-openapi.yml
  format: yaml
  label: MyFatoorah Invoicing API
  slug: myfatoorah-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-openapi.yml
- filename: myfatoorah-openapi.yml
  format: yaml
  label: MyFatoorah Payment Status API
  slug: myfatoorah-payment-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-openapi.yml
- filename: myfatoorah-openapi.yml
  format: yaml
  label: MyFatoorah Refunds API
  slug: myfatoorah-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-openapi.yml
- filename: myfatoorah-openapi.yml
  format: yaml
  label: MyFatoorah Embedded Sessions API
  slug: myfatoorah-embedded-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-openapi.yml
- filename: myfatoorah-openapi.yml
  format: yaml
  label: MyFatoorah Suppliers API
  slug: myfatoorah-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-openapi.yml
- filename: myfatoorah-openapi.yml
  format: yaml
  label: MyFatoorah Shipping API
  slug: myfatoorah-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-openapi.yml
- filename: myfatoorah-openapi.yml
  format: yaml
  label: MyFatoorah Recurring Payments API
  slug: myfatoorah-recurring-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-openapi.yml
- filename: myfatoorah-openapi.yml
  format: yaml
  label: MyFatoorah Webhooks API
  slug: myfatoorah-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-openapi.yml
description: ''
domains:
- dmarc: true
  dmarc_pct: 100
  dmarc_policy: reject
  dmarc_rua: mailto:info@myfatoorah.com
  domain: myfatoorah.com
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com include:mail.zendesk.com include:145768466.spf06.hubspotemail.net -all
hosts:
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: myfatoorah.com
  hsts: true
  hsts_max_age: 63072000
  http_status: 301
  https: true
  server: cloudflare
  tls_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: api.myfatoorah.com
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: true
  http_status: 200
  https: true
  server: cloudflare
  tls_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: apitest.myfatoorah.com
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: true
  http_status: 200
  https: true
  server: cloudflare
  tls_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: api-sa.myfatoorah.com
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: true
  http_status: 200
  https: true
  server: cloudflare
  tls_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: api-ae.myfatoorah.com
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: true
  http_status: 200
  https: true
  server: cloudflare
  tls_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1
kind: domain-security
layout: security
method: probed
name: Myfatoorah Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyFatoorah, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS; 5 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MyFatoorah
provider_slug: myfatoorah
slug: myfatoorah-domain-security
source_filename: myfatoorah-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myfatoorah.com\n  https: true\n  http_status: 301\n  tls_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  server: cloudflare\n- host: api.myfatoorah.com\n  https: true\n  http_status: 200\n  tls_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: true\n  server: cloudflare\n- host: apitest.myfatoorah.com\n  https: true\n  http_status: 200\n  tls_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: true\n  server: cloudflare\n- host: api-sa.myfatoorah.com\n  https: true\n  http_status: 200\n  tls_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1\n  cert_expires: Mar 19 23:59:59 2027\
  \ GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: true\n  server: cloudflare\n- host: api-ae.myfatoorah.com\n  https: true\n  http_status: 200\n  tls_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: true\n  server: cloudflare\ndomains:\n- domain: myfatoorah.com\n  spf: true\n  spf_record: 'v=spf1 include:spf.protection.outlook.com include:mail.zendesk.com include:145768466.spf06.hubspotemail.net -all'\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_pct: 100\n  dmarc_rua: 'mailto:info@myfatoorah.com'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/security/myfatoorah-domain-security.yml
summary_line: HSTS · DMARC
tags:
- Payments
- Payment Gateway
- Kuwait
- GCC
- MENA
- KNET
- mada
- Benefit
- Invoices
- Cards
- Fintech
---
