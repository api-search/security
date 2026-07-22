---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: magnific.ai
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: magnific.com
  spf: true
hosts:
- cert_expires: Sep 23 15:22:29 2026 GMT
  host: magnific.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 17:35:09 2026 GMT
  host: www.magnific.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Magnific Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Magnific, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Magnific
provider_slug: magnific-ai
slug: magnific-ai-domain-security
source_filename: magnific-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: magnific.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 15:22:29 2026 GMT\n  hsts: null\n- host: www.magnific.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 17:35:09 2026 GMT\n  hsts: null\ndomains:\n- domain: magnific.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: magnific.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magnific-ai/refs/heads/main/security/magnific-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Artificial Intelligence
- Image Upscaling
- Image Enhancement
- Generative AI
- Image Generation
- Computer Vision
- Creative Tools
- Relight
- Style Transfer
- Text To Image
- Freepik
- Spain
---
