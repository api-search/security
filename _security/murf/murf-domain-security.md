---
api_specs:
- filename: murf-openapi.yml
  format: yaml
  label: Murf API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/murf/refs/heads/main/openapi/murf-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: murf.ai
  spf: true
hosts:
- cert_expires: Mar 15 23:59:59 2027 GMT
  host: murf.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: api.murf.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: global.api.murf.ai
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Murf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Murf, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Murf
provider_slug: murf
slug: murf-domain-security
source_filename: murf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: murf.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.murf.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: null\n- host: global.api.murf.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: murf.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/murf/refs/heads/main/security/murf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Voice
- TTS
- Voiceover
- Dubbing
- Audio
- Realtime
---
