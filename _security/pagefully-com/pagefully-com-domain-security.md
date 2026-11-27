---
api_specs:
- filename: pagefully-com-openapi-generated.yml
  format: yaml
  label: Pagefully API
  slug: pagefully-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagefully-com/openapi/_ae-authored/pagefully-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pagefully.com
  spf: true
hosts:
- cert_expires: Jan  4 22:40:08 2027 GMT
  host: pagefully.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pagefully Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pagefully, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pagefully
provider_slug: pagefully-com
slug: pagefully-com-domain-security
source_filename: pagefully-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pagefully.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 22:40:08 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pagefully.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/pagefully-com/security/pagefully-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mobile
- App Store
- Marketing
- iOS
- Custom Pages
---
