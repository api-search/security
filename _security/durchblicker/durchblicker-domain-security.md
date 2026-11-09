---
description: ''
domains:
- caa:
  - 0 iodef "mailto:certviolations@durchblicker.at"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: durchblicker.at
  spf: true
hosts:
- cert_expires: Jan 11 01:32:43 2027 GMT
  host: durchblicker.at
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Durchblicker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Durchblicker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Durchblicker
provider_slug: durchblicker
slug: durchblicker-domain-security
source_filename: durchblicker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: durchblicker.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 01:32:43 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: durchblicker.at\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:certviolations@durchblicker.at\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/durchblicker/security/durchblicker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Finance
- Comparison
- Austria
---
