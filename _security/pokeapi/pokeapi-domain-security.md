---
api_specs:
- filename: pokeapi-openapi.yml
  format: yaml
  label: PokéAPI REST API v2
  slug: pokeapi-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pokeapi/refs/heads/main/openapi/pokeapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pokeapi.co
  spf: true
hosts:
- cert_expires: Sep  6 22:36:37 2026 GMT
  host: pokeapi.co
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 22:36:37 2026 GMT
  host: beta.pokeapi.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pokeapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PokéAPI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PokéAPI
provider_slug: pokeapi
slug: pokeapi-domain-security
source_filename: pokeapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pokeapi.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 22:36:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: beta.pokeapi.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 22:36:37 2026 GMT\n  hsts: null\ndomains:\n- domain: pokeapi.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pokeapi/refs/heads/main/security/pokeapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Pokémon
- Open Source
- Open Data
- REST
- GraphQL
- Gaming
- Educational
- Community
---
