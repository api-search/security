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
  dmarc: false
  dnssec: false
  domain: azul.cr
  spf: false
hosts:
- cert_expires: Jan 15 06:11:57 2027 GMT
  host: azul.cr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Azul CR Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azul CR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Azul CR
provider_slug: azul-cr
slug: azul-cr-domain-security
source_filename: azul-cr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: azul.cr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 06:11:57 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: azul.cr\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/azul-cr/security/azul-cr-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Directory
- WhatsApp
- Costa-Rica
- Business
- Marketplace
---
