---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fdb4.io
  spf: false
hosts:
- cert_expires: Jan  5 00:59:24 2027 GMT
  host: fdb4.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fdb4 Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FDB4, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: FDB4
provider_slug: fdb4-io
slug: fdb4-io-domain-security
source_filename: fdb4-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fdb4.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 00:59:24 2027 GMT\n  hsts: false\ndomains:\n- domain: fdb4.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fdb4-io/security/fdb4-io-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Football
- Sports
- Database
- Free
---
