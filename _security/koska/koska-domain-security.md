---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: koska.jp
  spf: true
hosts:
- cert_expires: Oct 10 19:43:52 2026 GMT
  host: koska.jp
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 22:29:29 2026 GMT
  host: vscribe.koska.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Koska Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Koska, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Koska
provider_slug: koska
slug: koska-domain-security
source_filename: koska-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: koska.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 19:43:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: vscribe.koska.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 22:29:29 2026 GMT\n  hsts: false\ndomains:\n- domain: koska.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koska/refs/heads/main/security/koska-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Manufacturing
- Cost Management
- Cost Accounting
- Industrial IoT
- IoT
- RFID
- Artificial Intelligence
- Voice Recognition
- Manufacturing Execution
- Japan
---
