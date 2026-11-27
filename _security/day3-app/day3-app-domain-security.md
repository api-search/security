---
api_specs:
- filename: day3-app-openapi-generated.yml
  format: yaml
  label: day3 API
  slug: day3-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/day3-app/openapi/_ae-authored/day3-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: day3.app
  spf: true
hosts:
- cert_expires: Jan 10 07:07:54 2027 GMT
  host: day3.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: day3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for day3, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: day3
provider_slug: day3-app
slug: day3-app-domain-security
source_filename: day3-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: day3.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 07:07:54 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: day3.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/day3-app/security/day3-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Marketing
- Transactional Email
- Software-as-a-Service
- Startup Tools
---
