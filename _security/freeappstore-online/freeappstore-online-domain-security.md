---
api_specs:
- filename: freeappstore-online-openapi-generated.yml
  format: yaml
  label: FreeAppStore API
  slug: freeappstore-online-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeappstore-online/openapi/_ae-authored/freeappstore-online-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: freeappstore.online
  spf: true
hosts:
- cert_expires: Jan 26 21:13:27 2027 GMT
  host: freeappstore.online
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FreeAppStore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FreeAppStore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FreeAppStore
provider_slug: freeappstore-online
slug: freeappstore-online-domain-security
source_filename: freeappstore-online-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freeappstore.online\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 21:13:27 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: freeappstore.online\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/freeappstore-online/security/freeappstore-online-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web App
- Free
- No Ads
- Productivity
- Finance
- Health and Fitness
- Learning
- Utilities
---
