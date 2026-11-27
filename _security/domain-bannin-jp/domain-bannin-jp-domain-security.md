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
  dmarc_policy: reject
  dnssec: false
  domain: domain-bannin.jp
  spf: true
hosts:
- cert_expires: Jan 21 16:00:21 2027 GMT
  host: domain-bannin.jp
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ドメイン番人 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ドメイン番人, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ドメイン番人
provider_slug: domain-bannin-jp
slug: domain-bannin-jp-domain-security
source_filename: domain-bannin-jp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: domain-bannin.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 16:00:21 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: domain-bannin.jp\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/domain-bannin-jp/security/domain-bannin-jp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Domain
- Security
- DNS
- Email
- SSL
---
