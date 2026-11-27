---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: imzala.net
  spf: true
hosts:
- cert_expires: Jan  4 15:15:44 2027 GMT
  host: imzala.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: imzala.net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for imzala.net, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: imzala.net
provider_slug: imzala-net
slug: imzala-net-domain-security
source_filename: imzala-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imzala.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 15:15:44 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: imzala.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/imzala-net/security/imzala-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal Tech
- Mediation
- Tax
- Trademarks
- Portal
---
