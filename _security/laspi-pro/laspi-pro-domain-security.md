---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: laspi.pro
  spf: false
hosts:
- cert_expires: Jan 12 08:31:37 2027 GMT
  host: laspi.pro
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Laspi Pro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Laspi Pro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Laspi Pro
provider_slug: laspi-pro
slug: laspi-pro-domain-security
source_filename: laspi-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: laspi.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 08:31:37 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: laspi.pro\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/laspi-pro/security/laspi-pro-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Marketing
- Social Media
- Small Business
- Content Generation
- Company
---
