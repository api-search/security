---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: brieform.app
  spf: true
hosts:
- cert_expires: Jan  1 19:27:06 2027 GMT
  host: brieform.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brieform App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brieform, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Brieform
provider_slug: brieform-app
slug: brieform-app-domain-security
source_filename: brieform-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brieform.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 19:27:06 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: brieform.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/brieform-app/security/brieform-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Form Builder
- Freelancers
- Agencies
- Web Forms
- No-Code
---
