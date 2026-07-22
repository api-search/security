---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: bunch.live
  spf: true
hosts:
- cert_expires: Sep 25 23:50:26 2026 GMT
  host: bunch.live
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Z1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Z1, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Z1
provider_slug: z1
slug: z1-domain-security
source_filename: z1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bunch.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:50:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bunch.live\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/z1/refs/heads/main/security/z1-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Consumer
- Gaming
- Social
- Video Chat
- Party Games
- Mobile
- Entertainment
---
