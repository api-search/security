---
api_specs:
- filename: cardmind-app-openapi-generated.yml
  format: yaml
  label: CardMind API
  slug: cardmind-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cardmind-app/openapi/_ae-authored/cardmind-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cardmind.app
  spf: true
hosts:
- cert_expires: Dec 21 07:40:02 2026 GMT
  host: cardmind.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CardMind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CardMind, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CardMind
provider_slug: cardmind-app
slug: cardmind-app-domain-security
source_filename: cardmind-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cardmind.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 07:40:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cardmind.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/cardmind-app/security/cardmind-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Market Intelligence
- Price Data
- Signals
- Ban Watch
- Deck Intelligence
---
