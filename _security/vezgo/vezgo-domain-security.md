---
api_specs:
- filename: vezgo-vezgo-api-openapi.yml
  format: yaml
  label: Vezgo API
  slug: vezgo-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vezgo/openapi/vezgo-vezgo-api-openapi.yml
- filename: vezgo-openapi-generated.yml
  format: yaml
  label: Vezgo API
  slug: vezgo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vezgo/openapi/_ae-authored/vezgo-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vezgo.com
  spf: true
hosts:
- cert_expires: Apr  2 23:59:59 2027 GMT
  host: vezgo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vezgo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vezgo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vezgo
provider_slug: vezgo
slug: vezgo-domain-security
source_filename: vezgo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vezgo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vezgo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/vezgo/security/vezgo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Data API
- Digital Assets
- Fintech
- Portfolio Tracking
---
