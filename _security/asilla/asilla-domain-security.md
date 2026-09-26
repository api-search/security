---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: asilla.com
  spf: false
hosts:
- cert_expires: Nov  6 18:56:35 2026 GMT
  host: en.asilla.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Asilla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asilla, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Asilla
provider_slug: asilla
slug: asilla-domain-security
source_filename: asilla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.asilla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 18:56:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: asilla.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asilla/refs/heads/main/security/asilla-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- Behavior-Recognition
- Security
- Video-Analytics
---
