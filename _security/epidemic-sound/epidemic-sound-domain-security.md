---
api_specs:
- filename: epidemic-sound-partner-content-api-openapi.yml
  format: yaml
  label: Epidemic Sound Partner Content API
  slug: epidemic-sound-partner-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epidemic-sound/refs/heads/main/openapi/epidemic-sound-partner-content-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: epidemicsound.com
  spf: true
hosts:
- cert_expires: Sep 25 18:42:48 2026 GMT
  host: www.epidemicsound.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 23:17:32 2026 GMT
  host: developers.epidemicsound.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 23:17:32 2026 GMT
  host: partner-content-api.epidemicsound.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Epidemic Sound Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Epidemic Sound, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Epidemic Sound
provider_slug: epidemic-sound
slug: epidemic-sound-domain-security
source_filename: epidemic-sound-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.epidemicsound.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 18:42:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.epidemicsound.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 23:17:32 2026 GMT\n  hsts: false\n- host: partner-content-api.epidemicsound.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 23:17:32 2026 GMT\n  hsts: null\ndomains:\n- domain: epidemicsound.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epidemic-sound/refs/heads/main/security/epidemic-sound-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Music
- Sound Effects
- Royalty-Free Music
- Audio
- Audio Licensing
- Soundtracking
- Sync Licensing
- Creators
- Video
- AI Voiceover
- Semantic Search
- MCP
---
