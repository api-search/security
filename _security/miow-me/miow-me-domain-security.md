---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: miow.me
  spf: true
hosts:
- cert_expires: Feb  3 15:50:13 2027 GMT
  host: miow.me
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: miow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for miow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: miow
provider_slug: miow-me
slug: miow-me-domain-security
source_filename: miow-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: miow.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 15:50:13 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: miow.me\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/miow-me/security/miow-me-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Website Builder
- Small Business
- AI Tools
- Subscription
- United Kingdom
---
