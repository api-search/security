---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: larabi.fr
  spf: true
hosts:
- cert_expires: Dec 16 06:25:30 2026 GMT
  host: larabi.fr
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: larabi-fr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for larabi-fr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: larabi-fr
provider_slug: larabi-fr
slug: larabi-fr-domain-security
source_filename: larabi-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: larabi.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 06:25:30 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: larabi.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/larabi-fr/security/larabi-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
