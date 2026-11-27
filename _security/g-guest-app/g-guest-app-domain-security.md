---
api_specs:
- filename: g-guest-app-openapi-generated.yml
  format: yaml
  label: G-Guest API
  slug: g-guest-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/g-guest-app/openapi/_ae-authored/g-guest-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: g-guest.app
  spf: true
hosts:
- cert_expires: Jan 24 12:11:25 2027 GMT
  host: g-guest.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: G-Guest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for G-Guest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: G-Guest
provider_slug: g-guest-app
slug: g-guest-app-domain-security
source_filename: g-guest-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: g-guest.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 12:11:25 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: g-guest.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/g-guest-app/security/g-guest-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Booking
- Software-as-a-Service
- Small Business
- Hospitality
---
