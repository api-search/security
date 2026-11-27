---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: marigold.page
  spf: false
hosts:
- cert_expires: Feb  8 02:53:08 2027 GMT
  host: marigold.page
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Marigold Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marigold, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Marigold
provider_slug: marigold-page
slug: marigold-page-domain-security
source_filename: marigold-page-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marigold.page\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 02:53:08 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: marigold.page\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/marigold-page/security/marigold-page-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Developer Tools
- Artificial Intelligence
- Code Review
- Open Source
- Productivity
---
