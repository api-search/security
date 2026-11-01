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
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getservd.me
  spf: true
hosts:
- cert_expires: Jan  4 16:52:21 2027 GMT
  host: getservd.me
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Getservd Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for getservd-me, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: getservd-me
provider_slug: getservd-me
slug: getservd-me-domain-security
source_filename: getservd-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getservd.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 16:52:21 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getservd.me\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/getservd-me/security/getservd-me-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- FoodTech
- Commerce
- SaaS
- Restaurants
---
