---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: freescout.net
  spf: true
hosts:
- cert_expires: Jan  7 23:42:11 2027 GMT
  host: freescout.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Freescout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FreeScout, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FreeScout
provider_slug: freescout
slug: freescout-domain-security
source_filename: freescout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freescout.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:42:11 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: freescout.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/freescout/security/freescout-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- HelpDesk
- OpenSource
- PHP
- Laravel
---
