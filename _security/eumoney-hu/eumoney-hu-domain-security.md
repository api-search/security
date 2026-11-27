---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eumoney.hu
  spf: true
hosts:
- cert_expires: Jan  5 20:20:15 2027 GMT
  host: eumoney.hu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EU Money Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EU Money, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EU Money
provider_slug: eumoney-hu
slug: eumoney-hu-domain-security
source_filename: eumoney-hu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eumoney.hu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 20:20:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eumoney.hu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/eumoney-hu/security/eumoney-hu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Grants
- EU
- Business
- Analytics
---
