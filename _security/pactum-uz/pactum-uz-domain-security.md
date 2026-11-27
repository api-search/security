---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pactum.uz
  spf: false
hosts:
- cert_expires: Feb 14 23:13:49 2027 GMT
  host: pactum.uz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pactum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pactum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Pactum
provider_slug: pactum-uz
slug: pactum-uz-domain-security
source_filename: pactum-uz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pactum.uz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:13:49 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pactum.uz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/pactum-uz/security/pactum-uz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal Services
- Uzbekistan
- Corporate Law
- Tax Consulting
- Business Support
---
