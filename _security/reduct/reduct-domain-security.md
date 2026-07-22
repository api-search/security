---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reduct.video
  spf: true
hosts:
- cert_expires: Sep  7 07:11:07 2026 GMT
  host: reduct.video
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reduct Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reduct, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Reduct
provider_slug: reduct
slug: reduct-domain-security
source_filename: reduct-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reduct.video\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 07:11:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: reduct.video\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reduct/refs/heads/main/security/reduct-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Applications
- Video
- Transcription
- Translation
- Redaction
- Video Editing
- Media
- Artificial Intelligence
---
