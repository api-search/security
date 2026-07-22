---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: farmwise.io
  spf: true
hosts:
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: farmwise.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Farmwise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Farmwise, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Farmwise
provider_slug: farmwise
slug: farmwise-domain-security
source_filename: farmwise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: farmwise.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: farmwise.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farmwise/refs/heads/main/security/farmwise-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Agriculture
- AgTech
- Robotics
- Artificial Intelligence
- Computer Vision
- Automation
---
