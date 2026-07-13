---
api_specs:
- filename: swapi-openapi.yml
  format: yaml
  label: SWAPI REST API (swapi.dev)
  slug: swapi-rest-api-swapidev
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swapi/refs/heads/main/openapi/swapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: swapi.dev
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: swapi.tech
  spf: true
hosts:
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: swapi.dev
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 15:57:50 2026 GMT
  host: www.swapi.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SWAPI - Star Wars API, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: SWAPI - Star Wars API
provider_slug: swapi
slug: swapi-domain-security
source_filename: swapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swapi.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: www.swapi.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 15:57:50 2026 GMT\n  hsts: null\ndomains:\n- domain: swapi.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: swapi.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swapi/refs/heads/main/security/swapi-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Star Wars
- Open Source
- Teaching API
- Public API
- REST
- GraphQL
- Entertainment
- Datasets
---
