---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: unity.com
  spf: true
hosts:
- cert_expires: Aug 19 23:59:59 2026 GMT
  host: unity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 07:00:23 2026 GMT
  host: cloud.unity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 07:00:23 2026 GMT
  host: dashboard.unity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unity Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unity, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Unity
provider_slug: unity-com
slug: unity-com-domain-security
source_filename: unity-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 23:59:59 2026 GMT\n  hsts: false\n- host: cloud.unity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 07:00:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dashboard.unity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 07:00:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: unity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unity-com/refs/heads/main/security/unity-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Time 3D
- Game Engine
- Gaming
- Multiplayer
- Cloud
- Live Operations
- Digital Twins
- XR
- ML-Agents
- Asset Pipeline
---
