---
api_specs:
- filename: api
  format: yaml
  label: Rick and Morty REST API
  slug: rick-and-morty-rest-api
  spec_type: OpenAPI
  url: https://rickandmortyapi.com/api
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rickandmortyapi.com
  spf: true
hosts:
- cert_expires: Aug 20 21:24:58 2026 GMT
  host: rickandmortyapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rickandmorty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rick and Morty API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rick and Morty API
provider_slug: rickandmorty
slug: rickandmorty-domain-security
source_filename: rickandmorty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rickandmortyapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 21:24:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rickandmortyapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rickandmorty/refs/heads/main/security/rickandmorty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Rick and Morty
- Characters
- Episodes
- Locations
- Entertainment
- GraphQL
- REST
- Free
- Open Source
---
