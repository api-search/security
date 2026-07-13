---
api_specs:
- filename: superheroes-openapi.yml
  format: yaml
  label: Superhero API
  slug: superhero-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superheroes/refs/heads/main/openapi/superheroes-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jsdelivr.net
  spf: false
hosts:
- cert_expires: Dec  5 14:48:47 2026 GMT
  host: cdn.jsdelivr.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superheroes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Superhero API (akabab), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Superhero API (akabab)
provider_slug: superheroes
slug: superheroes-domain-security
source_filename: superheroes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cdn.jsdelivr.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 14:48:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jsdelivr.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superheroes/refs/heads/main/security/superheroes-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Games And Comics
- Superheroes
- Comic Books
- Open Source
- Static API
- GitHub Pages
- Public APIs
---
