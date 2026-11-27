---
api_specs:
- filename: careleader-guide-openapi-generated.yml
  format: yaml
  label: Care Leader Guide API
  slug: careleader-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/careleader-guide/openapi/_ae-authored/careleader-guide-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: careleader.guide
  spf: false
hosts:
- cert_expires: Jan  1 07:34:14 2027 GMT
  host: careleader.guide
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Care Leader Guide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Care Leader Guide, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Care Leader Guide
provider_slug: careleader-guide
slug: careleader-guide-domain-security
source_filename: careleader-guide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: careleader.guide\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 07:34:14 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: careleader.guide\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/careleader-guide/security/careleader-guide-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Care
- Leadership
- Guides
- Community
- Healthcare
---
