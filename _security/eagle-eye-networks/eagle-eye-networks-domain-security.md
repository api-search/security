---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: een.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eagleeyenetworks.com
  spf: true
hosts:
- cert_expires: Sep 14 19:59:05 2026 GMT
  host: www.een.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 20:02:06 2026 GMT
  host: developer.eagleeyenetworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 20:10:47 2026 GMT
  host: api.eagleeyenetworks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eagle Eye Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eagle Eye Networks, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Eagle Eye Networks
provider_slug: eagle-eye-networks
slug: eagle-eye-networks-domain-security
source_filename: eagle-eye-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.een.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:59:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.eagleeyenetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 20:02:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.eagleeyenetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 20:10:47 2026 GMT\n  hsts: null\ndomains:\n- domain: een.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: eagleeyenetworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eagle-eye-networks/refs/heads/main/security/eagle-eye-networks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Video Surveillance
- Video Management
- Cloud Video
- Cameras
- Physical Security
- Video Analytics
- License Plate Recognition
- Streaming
- Webhooks
- OAuth
---
