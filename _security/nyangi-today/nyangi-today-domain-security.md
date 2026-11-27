---
api_specs:
- filename: nyangi-today-public-api-openapi.yml
  format: yaml
  label: 오늘냥이 Public API
  slug: nyangi-today-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nyangi-today/openapi/nyangi-today-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: nyangi.today
  spf: true
hosts:
- cert_expires: Feb 10 21:02:11 2027 GMT
  host: nyangi.today
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 오늘냥이 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 오늘냥이, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: 오늘냥이
provider_slug: nyangi-today
slug: nyangi-today-domain-security
source_filename: nyangi-today-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nyangi.today\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 21:02:11 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nyangi.today\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/nyangi-today/security/nyangi-today-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Community
- Cats
- Social
- Photo Sharing
- Korean
---
