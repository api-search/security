---
api_specs:
- filename: recur-tw-checkout-sessions-api-openapi.yml
  format: yaml
  label: Recur Checkout Sessions API
  slug: recur-tw-checkout-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recur-tw/openapi/recur-tw-checkout-sessions-api-openapi.yml
- filename: recur-tw-products-api-openapi.yml
  format: yaml
  label: Recur Products API
  slug: recur-tw-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recur-tw/openapi/recur-tw-products-api-openapi.yml
- filename: recur-tw-subscription-schedules-api-openapi.yml
  format: yaml
  label: Recur Subscription Schedules API
  slug: recur-tw-subscription-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recur-tw/openapi/recur-tw-subscription-schedules-api-openapi.yml
- filename: recur-tw-subscription-switching-api-openapi.yml
  format: yaml
  label: Recur Subscription Switching API
  slug: recur-tw-subscription-switching-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recur-tw/openapi/recur-tw-subscription-switching-api-openapi.yml
- filename: recur-tw-subscriptions-api-openapi.yml
  format: yaml
  label: Recur Subscriptions API
  slug: recur-tw-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recur-tw/openapi/recur-tw-subscriptions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: false
  domain: recur.tw
  spf: false
hosts:
- cert_expires: Dec 21 02:37:35 2026 GMT
  host: recur.tw
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Recur Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Recur, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Recur
provider_slug: recur-tw
slug: recur-tw-domain-security
source_filename: recur-tw-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: recur.tw\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 02:37:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: recur.tw\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/recur-tw/security/recur-tw-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Subscription
- Payments
- CreatorEconomy
- Taiwan
- SaaS
---
