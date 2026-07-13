---
api_specs:
- filename: swagger.json
  format: json
  label: Currents News API
  slug: currents-news-api
  spec_type: OpenAPI
  url: https://currentsapi.services/json/swagger.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: currentsapi.services
  spf: true
hosts:
- cert_expires: Aug 25 08:17:14 2026 GMT
  host: currentsapi.services
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 08:17:14 2026 GMT
  host: api.currentsapi.services
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Currentsapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Currents API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Currents API
provider_slug: currentsapi
slug: currentsapi-domain-security
source_filename: currentsapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: currentsapi.services\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 08:17:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.currentsapi.services\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 08:17:14 2026 GMT\n  hsts: null\ndomains:\n- domain: currentsapi.services\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/currentsapi/refs/heads/main/security/currentsapi-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- News
- Media
- Search
- REST
- Real-Time
---
