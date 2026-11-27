---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: false
  dnssec: false
  domain: englishtestcoach.com
  spf: true
hosts:
- cert_expires: Dec 22 06:58:17 2026 GMT
  host: englishtestcoach.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: English Test Coach Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for English Test Coach, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: English Test Coach
provider_slug: englishtestcoach-com
slug: englishtestcoach-com-domain-security
source_filename: englishtestcoach-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: englishtestcoach.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 06:58:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: englishtestcoach.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/englishtestcoach-com/security/englishtestcoach-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Education
- IELTS
- Writing
- Test Preparation
- English
---
