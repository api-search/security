---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ftir.fun
  spf: true
hosts:
- cert_expires: Feb  5 00:33:25 2027 GMT
  host: ftir.fun
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FTIR.fun Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FTIR.fun, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: FTIR.fun
provider_slug: ftir-fun
slug: ftir-fun-domain-security
source_filename: ftir-fun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ftir.fun\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 00:33:25 2027 GMT\n  hsts: null\ndomains:\n- domain: ftir.fun\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ftir-fun/security/ftir-fun-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Spectroscopy
- FTIR
- Artificial Intelligence
- Data
---
