---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 8i.com
  spf: true
hosts:
- cert_expires: Sep 21 18:49:42 2026 GMT
  host: 8i.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: player.8i.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 8I Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 8i, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 8i
provider_slug: 8i
slug: 8i-domain-security
source_filename: 8i-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 8i.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 18:49:42 2026 GMT\n  hsts: false\n- host: player.8i.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: 8i.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/8i/refs/heads/main/security/8i-domain-security.yml
summary_line: TLSv1.3
tags:
- Volumetric Video
- Holograms
- 3D
- Augmented Reality
- Virtual Reality
- WebXR
- Streaming
- Media
- Video
- Entertainment
- Company
---
