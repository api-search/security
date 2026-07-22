---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: elkroom.com
  spf: true
hosts:
- cert_expires: Aug 28 22:38:53 2026 GMT
  host: elkroom.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elkroom Co Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ELKROOM CO., LTD., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ELKROOM CO., LTD.
provider_slug: elkroom-co-ltd
slug: elkroom-co-ltd-domain-security
source_filename: elkroom-co-ltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elkroom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 22:38:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: elkroom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elkroom-co-ltd/refs/heads/main/security/elkroom-co-ltd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Gaming
- Mobile
- Consumer Apps
- Game Launcher
- AI Video
- Social Platform
- Android
- iOS
---
