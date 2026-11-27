---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: avizo.ro
  spf: true
hosts:
- cert_expires: Jan 17 21:57:42 2027 GMT
  host: avizo.ro
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Avizo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avizo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Avizo
provider_slug: avizo-ro
slug: avizo-ro-domain-security
source_filename: avizo-ro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avizo.ro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 21:57:42 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: avizo.ro\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/avizo-ro/security/avizo-ro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Alerts
- Compliance
- Document Management
- Romanian
- Automotive
---
