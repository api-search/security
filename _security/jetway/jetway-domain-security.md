---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nextravel.com
  spf: true
hosts:
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: nextravel.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jetway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jetway, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jetway
provider_slug: jetway
slug: jetway-domain-security
source_filename: jetway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nextravel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: nextravel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jetway/refs/heads/main/security/jetway-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Travel
- Corporate Travel
- Business Travel
- Expense Management
- Acquired
---
