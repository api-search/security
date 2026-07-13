---
api_specs:
- filename: play-ht-openapi.yml
  format: yaml
  label: PlayHT API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/play-ht/refs/heads/main/openapi/play-ht-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: play.ht
  spf: true
hosts:
- host: play.ht
  https: false
- cert_expires: Oct  2 18:45:09 2026 GMT
  host: docs.play.ht
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.play.ht
  https: false
kind: domain-security
layout: security
method: probed
name: Play Ht Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PlayHT, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PlayHT
provider_slug: play-ht
slug: play-ht-domain-security
source_filename: play-ht-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: play.ht\n  https: false\n- host: docs.play.ht\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:45:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.play.ht\n  https: false\ndomains:\n- domain: play.ht\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/play-ht/refs/heads/main/security/play-ht-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Voice
- TTS
- Voice Cloning
- Audio
- Realtime
---
