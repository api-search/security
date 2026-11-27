---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: deed.page
  spf: true
hosts:
- cert_expires: Jan 29 23:18:11 2027 GMT
  host: deed.page
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deed.page Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deed.page, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Deed.page
provider_slug: deed-page
slug: deed-page-domain-security
source_filename: deed-page-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deed.page\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:18:11 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: deed.page\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/deed-page/security/deed-page-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Hosting
- Artificial Intelligence
- Static Sites
- File Hosting
- Cloud
- Free Tier
---
