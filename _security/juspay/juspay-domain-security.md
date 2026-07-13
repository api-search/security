---
api_specs:
- filename: juspay-openapi.yml
  format: yaml
  label: Juspay Orders API
  slug: juspay-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juspay/refs/heads/main/openapi/juspay-openapi.yml
- filename: juspay-openapi.yml
  format: yaml
  label: Juspay Transactions API
  slug: juspay-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juspay/refs/heads/main/openapi/juspay-openapi.yml
- filename: juspay-openapi.yml
  format: yaml
  label: Juspay Session API
  slug: juspay-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juspay/refs/heads/main/openapi/juspay-openapi.yml
- filename: juspay-openapi.yml
  format: yaml
  label: Juspay Refunds API
  slug: juspay-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juspay/refs/heads/main/openapi/juspay-openapi.yml
- filename: juspay-openapi.yml
  format: yaml
  label: Juspay Customers API
  slug: juspay-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juspay/refs/heads/main/openapi/juspay-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: juspay.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: juspay.in
  spf: true
hosts:
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: juspay.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: api.juspay.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: sandbox.juspay.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Juspay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Juspay, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Juspay
provider_slug: juspay
slug: juspay-domain-security
source_filename: juspay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: juspay.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: false\n- host: api.juspay.in\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox.juspay.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: juspay.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: juspay.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/juspay/refs/heads/main/security/juspay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Orchestration
- Checkout
- India
- UPI
- Cards
- Payment Gateway
- Fintech
- HyperSDK
- Financial Infrastructure
---
