---
api_specs:
- filename: stigg-coupons-api-openapi.yml
  format: yaml
  label: Stigg Coupons API
  slug: stigg-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stigg/refs/heads/main/openapi/stigg-coupons-api-openapi.yml
- filename: stigg-customers-api-openapi.yml
  format: yaml
  label: Stigg Customers API
  slug: stigg-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stigg/refs/heads/main/openapi/stigg-customers-api-openapi.yml
- filename: stigg-entitlements-api-openapi.yml
  format: yaml
  label: Stigg Entitlements API
  slug: stigg-entitlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stigg/refs/heads/main/openapi/stigg-entitlements-api-openapi.yml
- filename: stigg-subscriptions-api-openapi.yml
  format: yaml
  label: Stigg Subscriptions API
  slug: stigg-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stigg/refs/heads/main/openapi/stigg-subscriptions-api-openapi.yml
- filename: stigg-usage-api-openapi.yml
  format: yaml
  label: Stigg Usage API
  slug: stigg-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stigg/refs/heads/main/openapi/stigg-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stigg.io
  spf: true
hosts:
- cert_expires: Sep 11 18:02:06 2026 GMT
  host: www.stigg.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 12:52:51 2026 GMT
  host: docs.stigg.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: api.stigg.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stigg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stigg, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stigg
provider_slug: stigg
slug: stigg-domain-security
source_filename: stigg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stigg.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 18:02:06 2026 GMT\n  hsts: false\n- host: docs.stigg.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:52:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.stigg.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: stigg.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stigg/refs/heads/main/security/stigg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- FinOps
- Pricing
- Billing
- Entitlements
- Usage-Based Billing
- Feature Flags
- Product-Led Growth
- Subscription
- Software-as-a-Service
- GraphQL
- REST
---
