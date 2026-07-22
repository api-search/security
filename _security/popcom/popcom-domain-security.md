---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: popcom.ai
  spf: false
hosts:
- cert_expires: Oct 11 05:32:32 2026 GMT
  host: www.popcom.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Popcom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PopCom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: PopCom
provider_slug: popcom
slug: popcom-domain-security
source_filename: popcom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.popcom.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 05:32:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: popcom.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/popcom/refs/heads/main/security/popcom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Automated Retail
- Vending
- Kiosk
- Retail Technology
- Computer Vision
- Analytics
- Robotics
---
