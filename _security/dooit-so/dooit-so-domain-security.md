---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dooit.so
  spf: true
hosts:
- cert_expires: Jan  9 10:17:42 2027 GMT
  host: dooit.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dooit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dooit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Dooit
provider_slug: dooit-so
slug: dooit-so-domain-security
source_filename: dooit-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dooit.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 10:17:42 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dooit.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/dooit-so/security/dooit-so-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Productivity
- Task Management
- Minimalist
- Web App
- Dooit
---
