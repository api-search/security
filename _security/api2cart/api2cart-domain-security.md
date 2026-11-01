---
api_specs:
- filename: api2cart-account-failed-webhooks-json-api-openapi.yml
  format: yaml
  label: Lexy Mayko Account.failed Webhooks.json API
  slug: api2cart-account-failed-webhooks-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api2cart/openapi/api2cart-account-failed-webhooks-json-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: api2cart.com
  spf: true
hosts:
- cert_expires: Dec 23 13:57:27 2026 GMT
  host: api2cart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Api2Cart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lexy Mayko, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lexy Mayko
provider_slug: api2cart
slug: api2cart-domain-security
source_filename: api2cart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api2cart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 13:57:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: api2cart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/api2cart/security/api2cart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Integration
- Software-as-a-Service
- Marketplace
---
