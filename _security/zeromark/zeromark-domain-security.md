---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zeromark.com
  spf: true
hosts:
- cert_expires: Sep 16 05:45:26 2026 GMT
  host: zeromark.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zeromark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZeroMark, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ZeroMark
provider_slug: zeromark
slug: zeromark-domain-security
source_filename: zeromark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zeromark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 05:45:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zeromark.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeromark/refs/heads/main/security/zeromark-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Defense
- Counter-Drone
- Counter-UAS
- Artificial Intelligence
- Targeting
- Command and Control
- Aerospace and Defense
- Hardware
---
