---
api_specs:
- filename: api
  format: yaml
  label: An API of Ice and Fire
  slug: an-api-of-ice-and-fire
  spec_type: OpenAPI
  url: https://www.anapioficeandfire.com/api
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: anapioficeandfire.com
  spf: true
hosts:
- cert_expires: Aug 31 08:03:04 2026 GMT
  host: anapioficeandfire.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 08:03:04 2026 GMT
  host: www.anapioficeandfire.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Game Of Thrones Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for An API of Ice and Fire, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: An API of Ice and Fire
provider_slug: game-of-thrones
slug: game-of-thrones-domain-security
source_filename: game-of-thrones-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anapioficeandfire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 08:03:04 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: www.anapioficeandfire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 08:03:04 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: anapioficeandfire.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/game-of-thrones/refs/heads/main/security/game-of-thrones-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Game of Thrones
- ASOIAF
- A Song of Ice and Fire
- Books
- Characters
- Houses
- Fantasy
- Entertainment
- Open API
- Free API
---
