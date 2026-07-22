---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: app-cm.co.jp
  spf: true
hosts:
- cert_expires: Sep  8 04:45:40 2026 GMT
  host: app-cm.co.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: App Cm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for App-CM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: App-CM
provider_slug: app-cm
slug: app-cm-domain-security
source_filename: app-cm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app-cm.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 04:45:40 2026 GMT\n  hsts: false\ndomains:\n- domain: app-cm.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/app-cm/refs/heads/main/security/app-cm-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Advertising
- Video Advertising
- AdTech
- Mobile
- Consumer Apps
- Platform
- Japan
---
