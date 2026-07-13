---
api_specs:
- filename: audiomack-data-api-openapi.yml
  format: yaml
  label: Audiomack Data API
  slug: audiomack-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audiomack/refs/heads/main/openapi/audiomack-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: audiomack.com
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: audiomack.com
  hsts: true
  hsts_max_age: 345600
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: creators.audiomack.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: www.audiomack.com
  hsts: true
  hsts_max_age: 345600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Audiomack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Audiomack, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Audiomack
provider_slug: audiomack
slug: audiomack-domain-security
source_filename: audiomack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: audiomack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 345600\n- host: creators.audiomack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: www.audiomack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 345600\ndomains:\n- domain: audiomack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audiomack/refs/heads/main/security/audiomack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Music
- Music Streaming
- Audio
- Podcasts
- Hip-Hop
- Rap
- Afrobeats
- Reggae
- Dancehall
- R&B
- Electronic
- Charts
- Playlists
- Discovery
- Creator Economy
- Independent Artists
---
