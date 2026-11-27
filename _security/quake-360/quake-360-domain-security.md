---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 360.net
  spf: true
hosts:
- cert_expires: May 26 23:59:59 2027 GMT
  host: quake.360.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Quake (Qihoo 360) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quake (Qihoo 360), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Quake (Qihoo 360)
provider_slug: quake-360
slug: quake-360-domain-security
source_filename: quake-360-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quake.360.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: May 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 360.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/quake-360/security/quake-360-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Security
- Asset Mapping
- Cybersecurity
- China
---
