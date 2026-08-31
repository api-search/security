---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ximilar.com
  spf: true
hosts:
- cert_expires: Oct  6 11:58:04 2026 GMT
  host: www.ximilar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:04:56 2026 GMT
  host: docs.ximilar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:04:56 2026 GMT
  host: api.ximilar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ximilar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ximilar, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ximilar
provider_slug: ximilar
slug: ximilar-domain-security
source_filename: ximilar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ximilar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 11:58:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ximilar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:04:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ximilar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:04:56 2026 GMT\n  hsts: null\ndomains:\n- domain: ximilar.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ximilar/refs/heads/main/security/ximilar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Computer Vision
- Image Recognition
- Visual Search
- Image Tagging
- Machine Learning
- Artificial Intelligence
- OCR
- Collectibles
- Fashion
- E-Commerce
- MCP
- Image Processing
---
