---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mriprices.fyi
  spf: true
hosts:
- cert_expires: Jan 18 07:44:51 2027 GMT
  host: mriprices.fyi
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MRIPrices Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MRIPrices, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MRIPrices
provider_slug: mriprices-fyi
slug: mriprices-fyi-domain-security
source_filename: mriprices-fyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mriprices.fyi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 07:44:51 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mriprices.fyi\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mriprices-fyi/security/mriprices-fyi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- MRI pricing
- hospital price transparency
- CMS data
---
