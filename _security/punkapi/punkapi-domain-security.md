---
api_specs:
- filename: punkapi-openapi.yml
  format: yaml
  label: Punk API — Beers
  slug: punk-api-beers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punkapi/refs/heads/main/openapi/punkapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: punkapi.com
  spf: false
hosts:
- host: punkapi.com
  https: false
- host: api.punkapi.com
  https: false
kind: domain-security
layout: security
method: probed
name: Punkapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Punk API, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Punk API
provider_slug: punkapi
slug: punkapi-domain-security
source_filename: punkapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: punkapi.com\n  https: false\n- host: api.punkapi.com\n  https: false\ndomains:\n- domain: punkapi.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/punkapi/refs/heads/main/security/punkapi-domain-security.yml
summary_line: DNSSEC
tags:
- Food And Drink
- Beer
- BrewDog
- DIY Dog
- Recipes
- Open Source
- Public APIs
- REST
- Deprecated
---
