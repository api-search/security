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
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: huebr.net
  spf: true
hosts:
- cert_expires: Jan 14 07:06:01 2027 GMT
  host: huebr.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: huebr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for huebr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: huebr
provider_slug: huebr-net
slug: huebr-net-domain-security
source_filename: huebr-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: huebr.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 07:06:01 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: huebr.net\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/huebr-net/security/huebr-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Prediction-Market
- Artificial Intelligence
- Analytics
- Odds
- Forecasting
---
