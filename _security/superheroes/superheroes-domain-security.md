---
api_specs:
- filename: superheroes-appearance-api-openapi.yml
  format: yaml
  label: Superhero API (akabab) Appearance API
  slug: superheroes-appearance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superheroes/refs/heads/main/openapi/superheroes-appearance-api-openapi.yml
- filename: superheroes-biography-api-openapi.yml
  format: yaml
  label: Superhero API (akabab) Biography API
  slug: superheroes-biography-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superheroes/refs/heads/main/openapi/superheroes-biography-api-openapi.yml
- filename: superheroes-characters-api-openapi.yml
  format: yaml
  label: Superhero API (akabab) Characters API
  slug: superheroes-characters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superheroes/refs/heads/main/openapi/superheroes-characters-api-openapi.yml
- filename: superheroes-connections-api-openapi.yml
  format: yaml
  label: Superhero API (akabab) Connections API
  slug: superheroes-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superheroes/refs/heads/main/openapi/superheroes-connections-api-openapi.yml
- filename: superheroes-images-api-openapi.yml
  format: yaml
  label: Superhero API (akabab) Images API
  slug: superheroes-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superheroes/refs/heads/main/openapi/superheroes-images-api-openapi.yml
- filename: superheroes-powerstats-api-openapi.yml
  format: yaml
  label: Superhero API (akabab) Powerstats API
  slug: superheroes-powerstats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superheroes/refs/heads/main/openapi/superheroes-powerstats-api-openapi.yml
- filename: superheroes-work-api-openapi.yml
  format: yaml
  label: Superhero API (akabab) Work API
  slug: superheroes-work-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superheroes/refs/heads/main/openapi/superheroes-work-api-openapi.yml
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
