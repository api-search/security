---
api_specs:
- filename: thefork-b2b-openapi.yml
  format: yaml
  label: TheFork B2B API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thefork/refs/heads/main/openapi/thefork-b2b-openapi.yml
- filename: thefork-pos-openapi.yml
  format: yaml
  label: TheFork POS API
  slug: pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thefork/refs/heads/main/openapi/thefork-pos-openapi.yml
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
name: Thefork Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TheFork, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TheFork
provider_slug: thefork
slug: thefork-domain-security
source_filename: thefork-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thefork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: null\n- host: docs.thefork.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.thefork.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: thefork.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: thefork.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thefork/refs/heads/main/security/thefork-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Reservations
- Booking
- Dining
- Point Of Sale
- Marketplace
---
