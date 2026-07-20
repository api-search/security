---
api_specs:
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Charges API
  slug: payjp-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Customers API
  slug: payjp-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Cards API
  slug: payjp-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Tokens API
  slug: payjp-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Plans API
  slug: payjp-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Subscriptions API
  slug: payjp-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Transfers API
  slug: payjp-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Statements & Balances API
  slug: payjp-statements-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Events & Webhooks API
  slug: payjp-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP 3D Secure API
  slug: payjp-three-d-secure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Platform API (Tenants)
  slug: payjp-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Account API
  slug: payjp-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
description: ''
domains:
- caa: []
  caa_note: No CAA records returned at probe time.
  dmarc: true
  dmarc_policy: none
  dmarc_record: v=DMARC1;p=none
  dnssec: false
  domain: pay.jp
hosts:
- cert_expires: Oct  1 02:53:48 2026 GMT
  cert_notBefore: Jul  3 02:53:49 2026 GMT
  host: pay.jp
  hsts: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 23:59:59 2027 GMT
  cert_notBefore: Jun 27 00:00:00 2026 GMT
  host: api.pay.jp
  hsts: true
  hsts_max_age: 86400
  http_status: 404
  https: true
  note: API root returns 404 by design; auth/paths required. HTTPS enforced.
  tls_version: TLSv1.3
- cert_expires: Jan 10 23:59:59 2027 GMT
  cert_notBefore: Jun 27 00:00:00 2026 GMT
  host: docs.pay.jp
  hsts: true
  hsts_max_age: 86400
  http_status: 200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Payjp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PAY.JP, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: PAY.JP
provider_slug: payjp
slug: payjp-domain-security
source_filename: payjp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + API hosts\nhosts:\n- host: pay.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_notBefore: Jul  3 02:53:49 2026 GMT\n  cert_expires: Oct  1 02:53:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  http_status: 200\n- host: api.pay.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_notBefore: Jun 27 00:00:00 2026 GMT\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\n  http_status: 404\n  note: API root returns 404 by design; auth/paths required. HTTPS enforced.\n- host: docs.pay.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_notBefore: Jun 27 00:00:00 2026 GMT\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\n  http_status: 200\ndomains:\n- domain: pay.jp\n  dnssec: false\n  caa: []\n  caa_note: No CAA records returned at probe time.\n  dmarc: true\n  dmarc_policy: none\n  dmarc_record: v=DMARC1;p=none\ntransport:\n  tls_only:\
  \ true\n  note: API is HTTPS-only (docs state HTTPS required); all probed hosts negotiated TLSv1.3.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/security/payjp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- FinTech
- Japan
- Credit Cards
- Subscriptions
- Tokenization
---
