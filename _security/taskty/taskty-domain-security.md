---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: taskty.com
  spf: false
hosts:
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: taskty.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Taskty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taskty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Taskty
provider_slug: taskty
slug: taskty-domain-security
source_filename: taskty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taskty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: taskty.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taskty/refs/heads/main/security/taskty-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Home Services
- Marketplace
- On-Demand
- Cleaning
- Maintenance
- Egypt
- Mobile App
---
