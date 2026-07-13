---
api_specs:
- filename: ron-swanson-quotes-openapi.yml
  format: yaml
  label: Ron Swanson Quotes API
  slug: ron-swanson-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ron-swanson-quotes/refs/heads/main/openapi/ron-swanson-quotes-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: herokuapp.com
  spf: false
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: ron-swanson-quotes.herokuapp.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ron Swanson Quotes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ron Swanson Quotes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Ron Swanson Quotes
provider_slug: ron-swanson-quotes
slug: ron-swanson-quotes-domain-security
source_filename: ron-swanson-quotes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ron-swanson-quotes.herokuapp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: herokuapp.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ron-swanson-quotes/refs/heads/main/security/ron-swanson-quotes-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Entertainment
- Television
- Parks and Recreation
- Quotes
- Open Source
- Public APIs
- Node.js
- TypeScript
- Heroku
- REST
---
