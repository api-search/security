---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: visual-layer.com
  spf: true
hosts:
- cert_expires: Oct 14 22:02:31 2026 GMT
  host: visual-layer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:15:21 2026 GMT
  host: docs.visual-layer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 14:11:08 2026 GMT
  host: app.visual-layer.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Visual Layer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Visual Layer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Visual Layer
provider_slug: visual-layer
slug: visual-layer-domain-security
source_filename: visual-layer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: visual-layer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 22:02:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.visual-layer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:15:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.visual-layer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 14:11:08 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: visual-layer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/visual-layer/refs/heads/main/security/visual-layer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Computer Vision
- Machine Learning
- Data Management
- Dataset Curation
- Unstructured Data
- Images
- Video
- Semantic Search
- AI
---
