---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: freewheel.com
  spf: true
hosts:
- cert_expires: Oct  3 20:16:05 2026 GMT
  host: www.freewheel.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 02:16:46 2026 GMT
  host: partners.freewheel.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freewheel Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FreeWheel Media, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FreeWheel Media
provider_slug: freewheel-media
slug: freewheel-media-domain-security
source_filename: freewheel-media-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.freewheel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:16:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: partners.freewheel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 02:16:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: freewheel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freewheel-media/refs/heads/main/security/freewheel-media-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- AdTech
- Streaming TV
- Video Advertising
- Programmatic
- Media
- Publisher Monetization
- Comcast
---
