---
api_specs:
- filename: index
  format: yaml
  label: BigOven Build API
  slug: bigoven-api
  spec_type: OpenAPI
  url: https://api2.bigoven.com/swagger/ui/index
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bigoven.com
  spf: true
hosts:
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: www.bigoven.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: api2.bigoven.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bigoven Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BigOven, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BigOven
provider_slug: bigoven
slug: bigoven-domain-security
source_filename: bigoven-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bigoven.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api2.bigoven.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: bigoven.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigoven/refs/heads/main/security/bigoven-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Recipes
- Meal Planning
- Grocery Lists
- Nutrition
- Food
- Cooking
---
