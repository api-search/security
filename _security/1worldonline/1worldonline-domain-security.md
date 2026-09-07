---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 1worldonline.com
  spf: true
hosts:
- cert_expires: Oct 13 06:20:07 2026 GMT
  host: 1worldonline.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 06:20:07 2026 GMT
  host: welcome.1worldonline.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 10:16:25 2026 GMT
  host: app-wleu.1worldonline.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: 1Worldonline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1World Online, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 1World Online
provider_slug: 1worldonline
slug: 1worldonline-domain-security
source_filename: 1worldonline-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 1worldonline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 06:20:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: welcome.1worldonline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 06:20:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app-wleu.1worldonline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 10:16:25 2026 GMT\n  hsts: null\ndomains:\n- domain: 1worldonline.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1worldonline/refs/heads/main/security/1worldonline-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Audience Engagement
- Polls
- Surveys
- Quizzes
- Loyalty
- Media
- Publishing
- Widgets
- Web3
---
