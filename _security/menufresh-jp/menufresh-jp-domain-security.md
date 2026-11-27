---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: menufresh.jp
  spf: true
hosts:
- cert_expires: Feb 13 15:08:49 2027 GMT
  host: menufresh.jp
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MenuFresh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MenuFresh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MenuFresh
provider_slug: menufresh-jp
slug: menufresh-jp-domain-security
source_filename: menufresh-jp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: menufresh.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 15:08:49 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: menufresh.jp\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/menufresh-jp/security/menufresh-jp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Food Tech
- Artificial Intelligence
- Restaurant Management
- Software-as-a-Service
- Japan
---
