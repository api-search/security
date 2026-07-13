---
api_specs:
- filename: marvel-openapi.yml
  format: yaml
  label: Marvel Comics API
  slug: marvel-comics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marvel/refs/heads/main/openapi/marvel-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: marvel.com
  spf: true
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: developer.marvel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: www.marvel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: gateway.marvel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marvel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marvel, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Marvel
provider_slug: marvel
slug: marvel-domain-security
source_filename: marvel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.marvel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: null\n- host: www.marvel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\n- host: gateway.marvel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: marvel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marvel/refs/heads/main/security/marvel-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Characters
- Comics
- Creators
- Entertainment
- Events
- Media
- Series
- Stories
---
