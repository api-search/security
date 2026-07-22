---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: photocert.co.uk
  spf: true
hosts:
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: photocert.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Photocert Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Photocert, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Photocert
provider_slug: photocert
slug: photocert-domain-security
source_filename: photocert-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: photocert.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: photocert.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/photocert/refs/heads/main/security/photocert-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Visual AI
- Image Certification
- Fraud Detection
- Insurance
- Insurtech
- Deepfake Detection
- Media Authentication
- Computer Vision
---
