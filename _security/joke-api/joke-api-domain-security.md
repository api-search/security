---
api_specs:
- filename: openapi.json
  format: json
  label: JokeAPI
  slug: joke-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Sv443-Network/JokeAPI/master/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: jokeapi.dev
  spf: false
hosts:
- cert_expires: Sep  6 15:51:56 2026 GMT
  host: jokeapi.dev
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 15:51:56 2026 GMT
  host: v2.jokeapi.dev
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Joke Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JokeAPI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: JokeAPI
provider_slug: joke-api
slug: joke-api-domain-security
source_filename: joke-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jokeapi.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 15:51:56 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: v2.jokeapi.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 15:51:56 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: jokeapi.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/joke-api/refs/heads/main/security/joke-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Jokes
- Humor
- Entertainment
- Programming Jokes
- Dark Humor
- Puns
- Free API
- Open Source
---
