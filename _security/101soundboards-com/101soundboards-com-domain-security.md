---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 101soundboards.com
  spf: true
hosts:
- cert_expires: Jan 15 21:28:41 2027 GMT
  host: 101soundboards.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 101Soundboards Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 101 Soundboards, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 101 Soundboards
provider_slug: 101soundboards-com
slug: 101soundboards-com-domain-security
source_filename: 101soundboards-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 101soundboards.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 21:28:41 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 101soundboards.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/101soundboards-com/security/101soundboards-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Audio
- soundboard
- Free
- Text-to-Speech
- Community
---
