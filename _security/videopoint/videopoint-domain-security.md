---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: touchpoints.cx
  spf: false
hosts:
- cert_expires: Sep 30 22:45:52 2026 GMT
  host: touchpoints.cx
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Videopoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VideoPoint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: VideoPoint
provider_slug: videopoint
slug: videopoint-domain-security
source_filename: videopoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: touchpoints.cx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 22:45:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: touchpoints.cx\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/videopoint/refs/heads/main/security/videopoint-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Shopify
- E-Commerce
- Video
- Conversion Optimization
- Shoppable Video
- AI
- Retail
---
