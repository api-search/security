---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jwplayer.com
  spf: true
hosts:
- cert_expires: Sep  1 19:32:54 2026 GMT
  host: jwplayer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 10:32:41 2026 GMT
  host: docs.jwplayer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: api.jwplayer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jwplayer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JW Player, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: JW Player
provider_slug: jwplayer
slug: jwplayer-domain-security
source_filename: jwplayer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jwplayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 19:32:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.jwplayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 10:32:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.jwplayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: jwplayer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jwplayer/refs/heads/main/security/jwplayer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video
- Streaming
- Media Management
- Live Streaming
- OTT
- Playlists
- Analytics
- DRM
- Advertising
- Webhooks
- Player
---
