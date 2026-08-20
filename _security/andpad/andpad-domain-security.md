---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: andpad.jp
  spf: true
hosts:
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: andpad.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: developer.andpad.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: api.andpad.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Andpad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ANDPAD, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ANDPAD
provider_slug: andpad
slug: andpad-domain-security
source_filename: andpad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: andpad.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: false\n- host: developer.andpad.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: false\n- host: api.andpad.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: andpad.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/andpad/refs/heads/main/security/andpad-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Technology
- Construction
- Construction Management
- Construction DX
- Software-as-a-Service
- Project Management
- Japan
---
