---
api_specs:
- filename: soundstripe-categories-api-openapi.yml
  format: yaml
  label: Soundstripe Categories API
  slug: soundstripe-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundstripe/refs/heads/main/openapi/soundstripe-categories-api-openapi.yml
- filename: soundstripe-playlists-api-openapi.yml
  format: yaml
  label: Soundstripe Playlists API
  slug: soundstripe-playlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundstripe/refs/heads/main/openapi/soundstripe-playlists-api-openapi.yml
- filename: soundstripe-private-playlists-api-openapi.yml
  format: yaml
  label: Soundstripe Private Playlists API
  slug: soundstripe-private-playlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundstripe/refs/heads/main/openapi/soundstripe-private-playlists-api-openapi.yml
- filename: soundstripe-songs-api-openapi.yml
  format: yaml
  label: Soundstripe Songs API
  slug: soundstripe-songs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundstripe/refs/heads/main/openapi/soundstripe-songs-api-openapi.yml
- filename: soundstripe-sound-effects-api-openapi.yml
  format: yaml
  label: Soundstripe Sound Effects API
  slug: soundstripe-sound-effects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundstripe/refs/heads/main/openapi/soundstripe-sound-effects-api-openapi.yml
- filename: soundstripe-supe-assets-api-openapi.yml
  format: yaml
  label: Soundstripe Supe Assets API
  slug: soundstripe-supe-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundstripe/refs/heads/main/openapi/soundstripe-supe-assets-api-openapi.yml
- filename: soundstripe-supe-search-api-openapi.yml
  format: yaml
  label: Soundstripe Supe Search API
  slug: soundstripe-supe-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundstripe/refs/heads/main/openapi/soundstripe-supe-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: soundstripe.com
  spf: true
hosts:
- cert_expires: Jan  6 15:14:08 2027 GMT
  host: www.soundstripe.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 21 02:52:56 2026 GMT
  host: docs.soundstripe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 15:14:08 2027 GMT
  host: api.soundstripe.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Soundstripe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Soundstripe, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Soundstripe
provider_slug: soundstripe
slug: soundstripe-domain-security
source_filename: soundstripe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.soundstripe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  6 15:14:08 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.soundstripe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 02:52:56 2026 GMT\n  hsts: null\n- host: api.soundstripe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  6 15:14:08 2027 GMT\n  hsts: null\ndomains:\n- domain: soundstripe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soundstripe/refs/heads/main/security/soundstripe-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Music
- Sound Effects
- Stock Video
- Royalty-Free
- Licensing
- Subscription
- Creators
- Content Creation
- Video Production
- Podcasting
- AI Music Supervisor
- Stems
---
