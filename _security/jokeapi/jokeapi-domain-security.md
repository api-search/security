---
api_specs:
- filename: jokeapi-openapi.yml
  format: yaml
  label: JokeAPI v2
  slug: jokeapi-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jokeapi/refs/heads/main/openapi/jokeapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: jokeapi.dev
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: sv443.net
  spf: true
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
- cert_expires: Sep 25 14:51:42 2026 GMT
  host: sv443.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jokeapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JokeAPI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: JokeAPI
provider_slug: jokeapi
slug: jokeapi-domain-security
source_filename: jokeapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jokeapi.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 15:51:56 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: v2.jokeapi.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 15:51:56 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: sv443.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 14:51:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jokeapi.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n- domain: sv443.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jokeapi/refs/heads/main/security/jokeapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Jokes
- Humor
- Entertainment
- Open Source
- REST API
- Games And Comics
- Public APIs
---
