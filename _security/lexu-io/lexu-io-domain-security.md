---
api_specs:
- filename: lexu-io-openapi-generated.yml
  format: yaml
  label: Lexu.io API
  slug: lexu-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexu-io/openapi/_ae-authored/lexu-io-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lexu.io
  spf: true
hosts:
- cert_expires: Feb 11 16:24:12 2027 GMT
  host: lexu.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lexu.io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lexu.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lexu.io
provider_slug: lexu-io
slug: lexu-io-domain-security
source_filename: lexu-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lexu.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 16:24:12 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lexu.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lexu-io/security/lexu-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Creative Studio
- Video Generation
- Image Generation
- Audio Generation
- Egypt
---
