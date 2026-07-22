---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shorebird.dev
  spf: true
hosts:
- cert_expires: Aug 25 17:47:19 2026 GMT
  host: shorebird.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shorebird Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shorebird, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Shorebird
provider_slug: shorebird
slug: shorebird-domain-security
source_filename: shorebird-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shorebird.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 17:47:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: shorebird.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shorebird/refs/heads/main/security/shorebird-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud Saas
- Flutter
- Code Push
- OTA Updates
- Mobile
- Mobile Apps
- Deployment
- CI/CD
- DevOps
---
