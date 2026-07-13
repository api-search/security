---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: babylonjs.com
  spf: true
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: www.babylonjs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: doc.babylonjs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: playground.babylonjs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Babylon Js Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Babylon.js, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Babylon.js
provider_slug: babylon-js
slug: babylon-js-domain-security
source_filename: babylon-js-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.babylonjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: false\n- host: doc.babylonjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: false\n- host: playground.babylonjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: babylonjs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/babylon-js/refs/heads/main/security/babylon-js-domain-security.yml
summary_line: TLSv1.3
tags:
- 3D
- Game Engine
- Rendering
- WebGL
- WebGPU
- WebXR
- TypeScript
- glTF
- Open Source
- Microsoft
---
