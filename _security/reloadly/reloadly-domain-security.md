---
api_specs:
- filename: reloadly-authentication-api-openapi.yml
  format: yaml
  label: Reloadly Authentication API
  slug: reloadly-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reloadly/refs/heads/main/openapi/reloadly-authentication-api-openapi.yml
- filename: reloadly-balance-api-openapi.yml
  format: yaml
  label: Reloadly Balance API
  slug: reloadly-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reloadly/refs/heads/main/openapi/reloadly-balance-api-openapi.yml
- filename: reloadly-discounts-api-openapi.yml
  format: yaml
  label: Reloadly Discounts API
  slug: reloadly-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reloadly/refs/heads/main/openapi/reloadly-discounts-api-openapi.yml
- filename: reloadly-operators-api-openapi.yml
  format: yaml
  label: Reloadly Operators API
  slug: reloadly-operators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reloadly/refs/heads/main/openapi/reloadly-operators-api-openapi.yml
- filename: reloadly-orders-api-openapi.yml
  format: yaml
  label: Reloadly Orders API
  slug: reloadly-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reloadly/refs/heads/main/openapi/reloadly-orders-api-openapi.yml
- filename: reloadly-products-api-openapi.yml
  format: yaml
  label: Reloadly Products API
  slug: reloadly-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reloadly/refs/heads/main/openapi/reloadly-products-api-openapi.yml
- filename: reloadly-top-ups-api-openapi.yml
  format: yaml
  label: Reloadly Top-Ups API
  slug: reloadly-top-ups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reloadly/refs/heads/main/openapi/reloadly-top-ups-api-openapi.yml
- filename: reloadly-transactions-api-openapi.yml
  format: yaml
  label: Reloadly Transactions API
  slug: reloadly-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reloadly/refs/heads/main/openapi/reloadly-transactions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: reloadly.com
  spf: true
hosts:
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: www.reloadly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: giftcards.reloadly.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: topups.reloadly.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Reloadly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reloadly, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Reloadly
provider_slug: reloadly
slug: reloadly-domain-security
source_filename: reloadly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reloadly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: false\n- host: giftcards.reloadly.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: null\n- host: topups.reloadly.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: reloadly.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reloadly/refs/heads/main/security/reloadly-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Gift Cards
- Payments
- Airtime
- Mobile Top-Up
- Rewards
- Incentives
---
