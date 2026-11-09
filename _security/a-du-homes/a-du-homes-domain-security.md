---
api_specs:
- filename: openapi.json
  format: json
  label: A-du API
  slug: a-du-api
  spec_type: OpenAPI
  url: https://a-du.homes/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: a-du.homes
  spf: true
hosts:
- cert_expires: Dec 24 16:36:25 2026 GMT
  host: a-du.homes
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: A Du Homes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for A-du, LLC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: A-du, LLC
provider_slug: a-du-homes
slug: a-du-homes-domain-security
source_filename: a-du-homes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: a-du.homes\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 16:36:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: a-du.homes\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/a-du-homes/security/a-du-homes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Property Management
- ADU
- Rentals
- Construction
---
