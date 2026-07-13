---
api_specs:
- filename: beatoven-composition-api-openapi.yml
  format: yaml
  label: Beatoven Composition API
  slug: beatoven-composition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beatoven/refs/heads/main/openapi/beatoven-composition-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: beatoven.ai
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: www.beatoven.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: public-api.beatoven.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beatoven Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beatoven.ai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Beatoven.ai
provider_slug: beatoven
slug: beatoven-domain-security
source_filename: beatoven-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.beatoven.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public-api.beatoven.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: beatoven.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beatoven/refs/heads/main/security/beatoven-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Artificial Intelligence
- Music
- Music Generation
- Generative Audio
- Text To Music
- Text To SFX
- Royalty-Free Music
- Background Music
- Video Creators
- Podcasts
- Stems
- Fairly Trained
- India
---
