---
api_specs:
- filename: ternivo-app-openapi-generated.yml
  format: yaml
  label: Ternivo API
  slug: ternivo-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ternivo-app/openapi/_ae-authored/ternivo-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: ternivo.app
  spf: true
hosts:
- cert_expires: Jan 10 12:33:17 2027 GMT
  host: ternivo.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ternivo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ternivo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ternivo
provider_slug: ternivo-app
slug: ternivo-app-domain-security
source_filename: ternivo-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ternivo.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 12:33:17 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ternivo.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/ternivo-app/security/ternivo-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Platform
- Privacy
- TripManagement
- Mobile
---
