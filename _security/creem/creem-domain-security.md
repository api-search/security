---
api_specs:
- filename: creem-openapi.yml
  format: yaml
  label: Creem Products API
  slug: products
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-openapi.yml
- filename: creem-openapi.yml
  format: yaml
  label: Creem Checkouts API
  slug: checkouts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-openapi.yml
- filename: creem-openapi.yml
  format: yaml
  label: Creem Customers API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-openapi.yml
- filename: creem-openapi.yml
  format: yaml
  label: Creem Subscriptions API
  slug: subscriptions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-openapi.yml
- filename: creem-openapi.yml
  format: yaml
  label: Creem Transactions API
  slug: transactions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-openapi.yml
- filename: creem-openapi.yml
  format: yaml
  label: Creem Discounts API
  slug: discounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-openapi.yml
- filename: creem-openapi.yml
  format: yaml
  label: Creem Licenses API
  slug: licenses
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-openapi.yml
- filename: creem-openapi.yml
  format: yaml
  label: Creem Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: creem.io
  spf: true
hosts:
- cert_expires: Oct  1 05:25:16 2026 GMT
  host: www.creem.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 08:54:21 2026 GMT
  host: docs.creem.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 14:22:56 2026 GMT
  host: api.creem.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Creem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Creem, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Creem
provider_slug: creem
slug: creem-domain-security
source_filename: creem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.creem.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 05:25:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.creem.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 08:54:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.creem.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 14:22:56 2026 GMT\n  hsts: false\ndomains:\n- domain: creem.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/security/creem-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Merchant of Record
- Subscriptions
- SaaS
- Billing
---
