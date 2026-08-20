---
api_specs:
- filename: clover-charges-api-openapi.yml
  format: yaml
  label: Clover CHARGES API
  slug: clover-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/openapi/clover-charges-api-openapi.yml
- filename: clover-checkout-api-openapi.yml
  format: yaml
  label: Clover CHECKOUT API
  slug: clover-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/openapi/clover-checkout-api-openapi.yml
- filename: clover-customers-api-openapi.yml
  format: yaml
  label: Clover CUSTOMERS API
  slug: clover-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/openapi/clover-customers-api-openapi.yml
- filename: clover-employees-api-openapi.yml
  format: yaml
  label: Clover EMPLOYEES API
  slug: clover-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/openapi/clover-employees-api-openapi.yml
- filename: clover-inventory-api-openapi.yml
  format: yaml
  label: Clover INVENTORY API
  slug: clover-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/openapi/clover-inventory-api-openapi.yml
- filename: clover-orders-api-openapi.yml
  format: yaml
  label: Clover ORDERS API
  slug: clover-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/openapi/clover-orders-api-openapi.yml
- filename: clover-payments-api-openapi.yml
  format: yaml
  label: Clover PAYMENTS API
  slug: clover-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/openapi/clover-payments-api-openapi.yml
- filename: clover-refunds-api-openapi.yml
  format: yaml
  label: Clover REFUNDS API
  slug: clover-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/openapi/clover-refunds-api-openapi.yml
- filename: clover-tokens-api-openapi.yml
  format: yaml
  label: Clover TOKENS API
  slug: clover-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/openapi/clover-tokens-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: clover.com
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: www.clover.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 26 12:47:22 2026 GMT
  host: docs.clover.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: api.clover.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Clover Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clover, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Clover
provider_slug: clover
slug: clover-domain-security
source_filename: clover-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clover.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.clover.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 12:47:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.clover.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: clover.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/security/clover-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Restaurant
- Point-of-Sale
- Payments
- Retail
- SMB
- Hardware
---
