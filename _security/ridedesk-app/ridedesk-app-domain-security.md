---
api_specs:
- filename: ridedesk-app-openapi-generated.yml
  format: yaml
  label: ridedesk-app API
  slug: ridedesk-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ridedesk-app/openapi/_ae-authored/ridedesk-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ridedesk.app
  spf: false
hosts:
- cert_expires: Jan 17 09:30:36 2027 GMT
  host: ridedesk.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ridedesk App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ridedesk-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: ridedesk-app
provider_slug: ridedesk-app
slug: ridedesk-app-domain-security
source_filename: ridedesk-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ridedesk.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 09:30:36 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ridedesk.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ridedesk-app/security/ridedesk-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Transportation
- Dispatch
- Booking
- SaaS
- API
---
