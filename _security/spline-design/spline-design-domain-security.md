---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: spline.design
  spf: true
hosts:
- cert_expires: Sep 13 17:42:56 2026 GMT
  host: spline.design
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spline Design Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spline, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Spline
provider_slug: spline-design
slug: spline-design-domain-security
source_filename: spline-design-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spline.design\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 17:42:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: spline.design\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spline-design/refs/heads/main/security/spline-design-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- 3D Design
- 3D Modeling
- Collaborative Design
- Interactive 3D
- Web Embed
- WebGL
- Animation
- Motion Design
- Materials
- Physics
- Particles
- SwiftUI
- Kotlin
- React
- React Three Fiber
- GLTF
- USDZ
- Webhooks
- Real-time API
- AI 3D Generation
- Design Tools
---
