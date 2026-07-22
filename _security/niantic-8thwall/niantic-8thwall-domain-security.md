---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 8thwall.org
  spf: false
hosts:
- cert_expires: Sep 30 08:07:49 2026 GMT
  host: 8thwall.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Niantic 8Thwall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 8th Wall, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: 8th Wall
provider_slug: niantic-8thwall
slug: niantic-8thwall-domain-security
source_filename: niantic-8thwall-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 8thwall.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 08:07:49 2026 GMT\n  hsts: false\ndomains:\n- domain: 8thwall.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/niantic-8thwall/refs/heads/main/security/niantic-8thwall-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Augmented Reality
- WebAR
- Web AR
- XR
- Extended Reality
- 3D
- SLAM
- World Tracking
- Image Targets
- Face Effects
- Sky Segmentation
- Niantic
- Niantic Spatial
- Open Source
- JavaScript SDK
- TypeScript
- A-Frame
- three.js
- PlayCanvas
- Babylon.js
---
