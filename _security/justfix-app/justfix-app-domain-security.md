---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: justfix.app
  spf: true
hosts:
- cert_expires: Feb  4 11:34:43 2027 GMT
  host: justfix.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: JustFix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JustFix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: JustFix
provider_slug: justfix-app
slug: justfix-app-domain-security
source_filename: justfix-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: justfix.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 11:34:43 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: justfix.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/justfix-app/security/justfix-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Home Services
- Renovation
- Plumbing
- Heating
- Smart Home
---
