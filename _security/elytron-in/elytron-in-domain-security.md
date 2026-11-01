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
  domain: elytron.in
  spf: true
hosts:
- cert_expires: Dec 31 02:25:49 2026 GMT
  host: elytron.in
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Elytron In Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for elytron-in, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: elytron-in
provider_slug: elytron-in
slug: elytron-in-domain-security
source_filename: elytron-in-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elytron.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 02:25:49 2026 GMT\n  hsts: false\ndomains:\n- domain: elytron.in\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/elytron-in/security/elytron-in-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- AI
- E-commerce
- SaaS
- Retail
---
