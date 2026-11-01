---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zucks.co.jp
  spf: false
hosts:
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: zucks.co.jp
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zucks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zucks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Zucks
provider_slug: zucks
slug: zucks-domain-security
source_filename: zucks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zucks.co.jp\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: zucks.co.jp\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/zucks/security/zucks-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
---
