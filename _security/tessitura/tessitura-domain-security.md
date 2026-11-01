---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tessitura.com
  spf: true
hosts:
- cert_expires: Jan 20 17:29:44 2027 GMT
  host: tessitura.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tessitura Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tessitura, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tessitura
provider_slug: tessitura
slug: tessitura-domain-security
source_filename: tessitura-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tessitura.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 17:29:44 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tessitura.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/tessitura/security/tessitura-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Arts
- Culture
- Nonprofit
- CRM
- Ticketing
---
