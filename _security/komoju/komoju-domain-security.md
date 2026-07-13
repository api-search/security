---
api_specs:
- filename: komoju-openapi.yml
  format: yaml
  label: KOMOJU Payments API
  slug: komoju-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komoju/refs/heads/main/openapi/komoju-openapi.yml
- filename: komoju-openapi.yml
  format: yaml
  label: KOMOJU Sessions API
  slug: komoju-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komoju/refs/heads/main/openapi/komoju-openapi.yml
- filename: komoju-openapi.yml
  format: yaml
  label: KOMOJU Tokens API
  slug: komoju-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komoju/refs/heads/main/openapi/komoju-openapi.yml
- filename: komoju-openapi.yml
  format: yaml
  label: KOMOJU Customers API
  slug: komoju-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komoju/refs/heads/main/openapi/komoju-openapi.yml
- filename: komoju-openapi.yml
  format: yaml
  label: KOMOJU Subscriptions API
  slug: komoju-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komoju/refs/heads/main/openapi/komoju-openapi.yml
- filename: komoju-openapi.yml
  format: yaml
  label: KOMOJU Payment Methods API
  slug: komoju-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komoju/refs/heads/main/openapi/komoju-openapi.yml
- filename: komoju-openapi.yml
  format: yaml
  label: KOMOJU Events API
  slug: komoju-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komoju/refs/heads/main/openapi/komoju-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: komoju.com
  spf: true
  spf_policy: ~all
hosts:
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: komoju.com
  hsts: false
  https: true
  note: API base host (https://komoju.com/api/v1). Apex returns an HTTP 308 redirect; no HSTS header observed on the redirect response.
  tls_version: TLSv1.3
- cert_expires: Sep 29 17:59:17 2026 GMT
  host: en.komoju.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 06:30:19 2026 GMT
  host: doc.komoju.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Komoju Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KOMOJU, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: KOMOJU
provider_slug: komoju
slug: komoju-domain-security
source_filename: komoju-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + API/doc hosts\nhosts:\n- host: komoju.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: false\n  note: API base host (https://komoju.com/api/v1). Apex returns an HTTP 308 redirect; no HSTS header observed on the redirect response.\n- host: en.komoju.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 17:59:17 2026 GMT\n  hsts: false\n- host: doc.komoju.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 06:30:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: komoju.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: '~all'\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/komoju/refs/heads/main/security/komoju-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Gateway
- Japan
- Konbini
- Cards
- PayPay
- Bank Transfer
- E-Money
- Checkout
- Fintech
---
