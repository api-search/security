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
  dnssec: false
  domain: fourthtake.com
  spf: true
hosts:
- cert_expires: Jan 27 21:29:02 2027 GMT
  host: fourthtake.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fourth Take Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fourth Take, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fourth Take
provider_slug: fourthtake-com
slug: fourthtake-com-domain-security
source_filename: fourthtake-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fourthtake.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 21:29:02 2027 GMT\n  hsts: false\ndomains:\n- domain: fourthtake.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fourthtake-com/security/fourthtake-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Media
- News
- Technology
- Politics
- Entertainment
- Company
---
