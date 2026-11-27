---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sharetribe.com
  spf: true
hosts:
- cert_expires: Jan 19 19:34:01 2027 GMT
  host: sharetribe.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sharetribe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sharetribe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sharetribe
provider_slug: sharetribe
slug: sharetribe-domain-security
source_filename: sharetribe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sharetribe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 19:34:01 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sharetribe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/sharetribe/security/sharetribe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketplace
- No-Code
- API-First
- Software-as-a-Service
- E-Commerce
---
