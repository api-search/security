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
  domain: massenversand.de
  spf: true
hosts:
- cert_expires: Jan 10 13:46:27 2027 GMT
  host: massenversand.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Massenversand Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Massenversand, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Massenversand
provider_slug: massenversand
slug: massenversand-domain-security
source_filename: massenversand-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: massenversand.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 13:46:27 2027 GMT\n  hsts: false\ndomains:\n- domain: massenversand.de\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/massenversand/security/massenversand-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- SMS
- Messaging
- API
- Marketing
- Germany
- Communication
---
