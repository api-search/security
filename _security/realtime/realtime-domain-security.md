---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ietf.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: whatwg.org
  spf: true
hosts:
- cert_expires: Oct  5 20:01:07 2026 GMT
  host: datatracker.ietf.org
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 02:20:30 2026 GMT
  host: html.spec.whatwg.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: webrtc.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Realtime Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Realtime, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Realtime
provider_slug: realtime
slug: realtime-domain-security
source_filename: realtime-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datatracker.ietf.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 20:01:07 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\n- host: html.spec.whatwg.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 23 02:20:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: webrtc.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ietf.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: whatwg.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realtime/refs/heads/main/security/realtime-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Realtime
- WebSocket
- WebRTC
- Server-Sent Events
- MQTT
- Push Notifications
- Pub Sub
- Presence
- Signaling
- Topic
---
