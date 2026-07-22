---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: medivis.com
  spf: true
hosts:
- cert_expires: Sep 27 21:13:13 2026 GMT
  host: medivis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Medivis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Medivis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Medivis
provider_slug: medivis
slug: medivis-domain-security
source_filename: medivis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: medivis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 21:13:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: medivis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medivis/refs/heads/main/security/medivis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hardware
- Healthcare
- Augmented Reality
- Surgical Navigation
- Medical Imaging
- Medical Education
- Health Technology
---
