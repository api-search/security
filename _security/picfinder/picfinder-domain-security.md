---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: picfinder.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: diffusionmaster.com
  spf: false
hosts:
- cert_expires: Aug 31 07:55:45 2026 GMT
  host: picfinder.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 16:40:22 2026 GMT
  host: ws-api.diffusionmaster.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Picfinder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PicFinder, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PicFinder
provider_slug: picfinder
slug: picfinder-domain-security
source_filename: picfinder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: picfinder.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 07:55:45 2026 GMT\n  hsts: null\n- host: ws-api.diffusionmaster.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 16:40:22 2026 GMT\n  hsts: null\ndomains:\n- domain: picfinder.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: diffusionmaster.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/picfinder/refs/heads/main/security/picfinder-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Image Generation
- Generative AI
- Text to Image
- Image to Image
- Developer Tools
- SDK
- WebSocket
---
