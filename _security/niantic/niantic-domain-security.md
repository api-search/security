---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: nianticlabs.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: nianticspatial.com
  spf: true
hosts:
- cert_expires: Oct 12 23:48:45 2026 GMT
  host: nianticlabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 21:19:29 2026 GMT
  host: www.nianticspatial.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Niantic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Niantic, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Niantic
provider_slug: niantic
slug: niantic-domain-security
source_filename: niantic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nianticlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:48:45 2026 GMT\n  hsts: false\n- host: www.nianticspatial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 21:19:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nianticlabs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: nianticspatial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/niantic/refs/heads/main/security/niantic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Geospatial
- Augmented Reality
- Computer Vision
- Visual Positioning
- Spatial Computing
- SDK
- Physical AI
- Robotics
---
