---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kosmik.app
  spf: true
hosts:
- cert_expires: Sep 23 08:17:16 2026 GMT
  host: www.kosmik.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kosmik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kosmik, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kosmik
provider_slug: kosmik
slug: kosmik-domain-security
source_filename: kosmik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kosmik.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 08:17:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kosmik.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kosmik/refs/heads/main/security/kosmik-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consumer
- Productivity
- Visual Collaboration
- Infinite Canvas
- Moodboard
- Personal Knowledge Management
- Artificial Intelligence
- Local First
- Sunset
---
