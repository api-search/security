---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: insta360.com
  spf: true
hosts:
- cert_expires: Sep  5 09:04:33 2026 GMT
  host: insta360.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Insta360 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Insta360, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Insta360
provider_slug: insta360
slug: insta360-domain-security
source_filename: insta360-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: insta360.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 09:04:33 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: insta360.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insta360/refs/heads/main/security/insta360-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer Technology
- Cameras
- Imaging
- 360 Video
- Action Cameras
- SDK
- Open Spherical Camera
- IoT
---
