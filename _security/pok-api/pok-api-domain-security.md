---
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
kind: domain-security
layout: security
method: probed
name: Pok Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pokéapi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pokéapi
provider_slug: pok-api
slug: pok-api-domain-security
source_filename: pok-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pokeapi.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 22:36:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: pokeapi.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pok-api/refs/heads/main/security/pok-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Games And Comics
- Public APIs
---
