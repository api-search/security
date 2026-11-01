---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: etchv.com
  spf: true
hosts:
- cert_expires: Dec  5 04:36:50 2026 GMT
  host: etchv.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Etchv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for etchv, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: etchv
provider_slug: etchv
slug: etchv-domain-security
source_filename: etchv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: etchv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 04:36:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: etchv.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/etchv/security/etchv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Watermarking
- Media
- Security
- Developer Tools
---
