---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: feather.computer
  spf: false
hosts:
- cert_expires: Dec 13 06:24:44 2026 GMT
  host: feather.computer
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Feather Computers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Feather Computers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Feather Computers
provider_slug: feather-computers
slug: feather-computers-domain-security
source_filename: feather-computers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: feather.computer\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 06:24:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: feather.computer\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/feather-computers/security/feather-computers-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- Email
- Productivity
- SaaS
---
