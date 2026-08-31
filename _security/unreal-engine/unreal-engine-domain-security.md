---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: unrealengine.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: epicgames.com
  spf: true
hosts:
- cert_expires: Sep 28 17:56:33 2026 GMT
  host: www.unrealengine.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 01:58:57 2026 GMT
  host: dev.epicgames.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unreal Engine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unreal Engine, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Unreal Engine
provider_slug: unreal-engine
slug: unreal-engine-domain-security
source_filename: unreal-engine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unrealengine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 17:56:33 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: dev.epicgames.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 01:58:57 2026 GMT\n  hsts: false\ndomains:\n- domain: unrealengine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: epicgames.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unreal-engine/refs/heads/main/security/unreal-engine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- 3D
- Blueprint
- C++
- Game Development
- Game Engine
- Pixel Streaming
- Plugin
- Real-Time
- Rendering
- RHI
- SDK
- Unreal Engine
- WebRTC
---
