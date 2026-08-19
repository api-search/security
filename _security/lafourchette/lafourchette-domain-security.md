---
api_specs:
- filename: lafourchette-b2b-api-openapi.yml
  format: yaml
  label: TheFork B2B API
  slug: thefork-b2b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lafourchette/refs/heads/main/openapi/lafourchette-b2b-api-openapi.yml
- filename: lafourchette-pos-api-openapi.yml
  format: yaml
  label: TheFork POS API v1
  slug: thefork-pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lafourchette/refs/heads/main/openapi/lafourchette-pos-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: thefork.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: thefork.io
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: www.thefork.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: docs.thefork.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: api.thefork.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lafourchette Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LaFourchette, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LaFourchette
provider_slug: lafourchette
slug: lafourchette-domain-security
source_filename: lafourchette-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thefork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: null\n- host: docs.thefork.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.thefork.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: thefork.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: thefork.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lafourchette/refs/heads/main/security/lafourchette-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Restaurants
- Reservations
- Booking
- Hospitality
- Point of Sale
- Reviews
- Marketplace
- Travel and Dining
- Webhooks
- France
---
