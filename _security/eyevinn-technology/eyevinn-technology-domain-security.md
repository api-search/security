---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eyevinn.se
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: osaas.io
  spf: true
hosts:
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: www.eyevinn.se
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: docs.osaas.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: api.osaas.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eyevinn Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eyevinn Technology, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Eyevinn Technology
provider_slug: eyevinn-technology
slug: eyevinn-technology-domain-security
source_filename: eyevinn-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eyevinn.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: false\n- host: docs.osaas.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: false\n- host: api.osaas.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: eyevinn.se\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: osaas.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eyevinn-technology/refs/heads/main/security/eyevinn-technology-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Ad Insertion
- Broadcast Intercom
- Channel Engine
- CMAF
- DASH
- FAST Channels
- FFmpeg
- HLS
- Live Streaming
- Media Over QUIC
- Open Source
- Open Source Cloud
- OSC
- Player Analytics
- REST
- SRT
- SSAI
- Sweden
- Transcoding
- Video Infrastructure
- VOD2Live
- WebRTC
- WHEP
- WHIP
---
