---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sendcutsend.com
  spf: true
hosts:
- cert_expires: Oct 16 06:33:15 2026 GMT
  host: sendcutsend.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sendcutsend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SendCutSend, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SendCutSend
provider_slug: sendcutsend
slug: sendcutsend-domain-security
source_filename: sendcutsend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sendcutsend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 06:33:15 2026 GMT\n  hsts: false\ndomains:\n- domain: sendcutsend.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendcutsend/refs/heads/main/security/sendcutsend-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Manufacturing
- Laser Cutting
- Sheet Metal Fabrication
- CNC Machining
- Waterjet Cutting
- Custom Manufacturing
- On-Demand Manufacturing
---
