---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: goldencorral.com
  spf: true
hosts:
- cert_expires: Jan 21 07:22:13 2027 GMT
  host: www.goldencorral.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Golden Corral Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Golden Corral, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Golden Corral
provider_slug: goldencorral
slug: goldencorral-domain-security
source_filename: goldencorral-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.goldencorral.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 07:22:13 2027 GMT\n  hsts: false\ndomains:\n- domain: goldencorral.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/goldencorral/security/goldencorral-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Restaurant
- Buffet
- Food Service
- Family Dining
---
