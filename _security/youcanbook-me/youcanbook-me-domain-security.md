---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: youcanbook.me
  spf: true
hosts:
- cert_expires: Nov 20 13:34:08 2026 GMT
  host: youcanbook.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Youcanbook Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for YouCanBook.me, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: YouCanBook.me
provider_slug: youcanbook-me
slug: youcanbook-me-domain-security
source_filename: youcanbook-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: youcanbook.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 13:34:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: youcanbook.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/youcanbook-me/refs/heads/main/security/youcanbook-me-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Scheduling
- Software-as-a-Service
- Automation
- Integration
---
