---
api_specs:
- filename: l1nk-website-openapi-generated.yml
  format: yaml
  label: L1NK API
  slug: l1nk-website-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/l1nk-website/openapi/_ae-authored/l1nk-website-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: l1nk.website
  spf: true
hosts:
- cert_expires: Dec 19 08:08:03 2026 GMT
  host: l1nk.website
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: L1NK Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for L1NK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: L1NK
provider_slug: l1nk-website
slug: l1nk-website-domain-security
source_filename: l1nk-website-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: l1nk.website\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 08:08:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: l1nk.website\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/l1nk-website/security/l1nk-website-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Short Links
- URL Shorteners
- Analytics
- QR Codes
- AI Integration
---
