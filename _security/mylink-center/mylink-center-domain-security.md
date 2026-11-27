---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: mylink.center
  spf: false
hosts:
- cert_expires: Jan  3 05:35:29 2027 GMT
  host: mylink.center
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Link Center Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Link Center, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Link Center
provider_slug: mylink-center
slug: mylink-center-domain-security
source_filename: mylink-center-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mylink.center\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 05:35:29 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mylink.center\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mylink-center/security/mylink-center-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- QR Codes
- Short Links
- Dynamic URLs
- Analytics
- Pay-as-you-go
---
