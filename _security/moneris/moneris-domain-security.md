---
api_specs:
- filename: moneris-unified-api-openapi.json
  format: json
  label: Moneris Payments API
  slug: moneris-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-unified-api-openapi.json
- filename: moneris-unified-api-openapi.json
  format: json
  label: Moneris Payment Methods API
  slug: moneris-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-unified-api-openapi.json
- filename: moneris-unified-api-openapi.json
  format: json
  label: Moneris Refunds API
  slug: moneris-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-unified-api-openapi.json
- filename: moneris-unified-api-openapi.json
  format: json
  label: Moneris Subscriptions API
  slug: moneris-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-unified-api-openapi.json
- filename: moneris-unified-api-openapi.json
  format: json
  label: Moneris Customers API
  slug: moneris-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-unified-api-openapi.json
- filename: moneris-unified-api-openapi.json
  format: json
  label: Moneris 3-D Secure Authentication API
  slug: moneris-3d-secure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-unified-api-openapi.json
- filename: moneris-unified-api-openapi.json
  format: json
  label: Moneris Kount Risk Inquiry API
  slug: moneris-kount-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-unified-api-openapi.json
- filename: moneris-unified-api-openapi.json
  format: json
  label: Moneris Merchant Onboarding API
  slug: moneris-merchant-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-unified-api-openapi.json
- filename: moneris-unified-api-openapi.json
  format: json
  label: Moneris Multi-Currency Pricing API
  slug: moneris-multi-currency-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-unified-api-openapi.json
- filename: moneris-unified-api-openapi.json
  format: json
  label: Moneris Disputes API
  slug: moneris-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneris/refs/heads/main/openapi/moneris-unified-api-openapi.json
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
- Financial Services
- Payments
- Payment Processing
- Card Payments
- Merchant Services
- Acquiring
- Canada
- Fintech
- Infrastructure
---
