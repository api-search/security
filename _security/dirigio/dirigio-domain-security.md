---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dirigio.jp
  spf: false
hosts:
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: dirigio.jp
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dirigio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dirigio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Dirigio
provider_slug: dirigio
slug: dirigio-domain-security
source_filename: dirigio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dirigio.jp\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: dirigio.jp\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dirigio/security/dirigio-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- RestaurantTech
- Mobile Ordering
- Japan
- Platform
---
