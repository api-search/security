---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lighthouse.app
  spf: true
hosts:
- cert_expires: Dec  6 14:56:24 2026 GMT
  host: lighthouse.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lighthouse App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lighthouse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lighthouse
provider_slug: lighthouse-app
slug: lighthouse-app-domain-security
source_filename: lighthouse-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lighthouse.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 14:56:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lighthouse.app\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lighthouse-app/security/lighthouse-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- RealEstate
- FinTech
- Rentals
- Cashback
---
