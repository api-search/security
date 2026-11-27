---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nomok.app
  spf: false
hosts:
- cert_expires: Jan 11 11:29:54 2027 GMT
  host: nomok.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nomok Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nomok, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Nomok
provider_slug: nomok-app
slug: nomok-app-domain-security
source_filename: nomok-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nomok.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 11:29:54 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nomok.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/nomok-app/security/nomok-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- NameCheck
- Digital Identity
- Entrepreneurship
---
