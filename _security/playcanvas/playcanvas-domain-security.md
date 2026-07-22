---
api_specs:
- filename: playcanvas-rest-openapi.yml
  format: yaml
  label: PlayCanvas REST API
  slug: playcanvas-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playcanvas/refs/heads/main/openapi/playcanvas-rest-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: playcanvas.com
  spf: true
hosts:
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: playcanvas.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Playcanvas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PlayCanvas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: PlayCanvas
provider_slug: playcanvas
slug: playcanvas-domain-security
source_filename: playcanvas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: playcanvas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: playcanvas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playcanvas/refs/heads/main/security/playcanvas-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- 3D
- Game Engine
- WebGL
- WebGPU
- Graphics
- Developer Tools
- Gaussian Splatting
- Rendering
---
