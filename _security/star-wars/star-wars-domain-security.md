---
api_specs:
- filename: star-wars-openapi.json
  format: json
  label: Star Wars REST API
  slug: star-wars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/star-wars/refs/heads/main/openapi/star-wars-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: swapi.info
  spf: false
hosts:
- cert_expires: Oct  3 12:07:58 2026 GMT
  host: swapi.info
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Star Wars Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Star Wars API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Star Wars API
provider_slug: star-wars
slug: star-wars-domain-security
source_filename: star-wars-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swapi.info\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 12:07:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: swapi.info\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/star-wars/refs/heads/main/security/star-wars-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Star Wars
- Science Fiction
- Entertainment
- Films
- Characters
- Planets
- Starships
- Vehicles
- Species
- Open Source
---
