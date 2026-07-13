---
api_specs:
- filename: uber-eats-openapi.yml
  format: yaml
  label: Uber Eats Store API
  slug: store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber-eats/refs/heads/main/openapi/uber-eats-openapi.yml
- filename: uber-direct-openapi.yml
  format: yaml
  label: Uber Direct (Deliveries) API
  slug: uber-direct
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uber-eats/refs/heads/main/openapi/uber-direct-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uber.com
  spf: true
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: www.uber.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: developer.uber.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: api.uber.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uber Eats Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uber Eats, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Uber Eats
provider_slug: uber-eats
slug: uber-eats-domain-security
source_filename: uber-eats-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uber.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: null\n- host: developer.uber.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: null\n- host: api.uber.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: uber.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uber-eats/refs/heads/main/security/uber-eats-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Uber Eats
- Uber Direct
- Food Delivery
- Last-Mile Logistics
- Restaurants
- Menus
- Orders
- Fulfillment
- Courier
- OAuth2
---
