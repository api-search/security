---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: won.ai
  spf: true
hosts:
- cert_expires: Jan 20 01:54:26 2027 GMT
  host: won.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Won Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WON, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: WON
provider_slug: won
slug: won-domain-security
source_filename: won-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: won.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 01:54:26 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: won.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/won/security/won-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Advisory
- Business-Design
- Retail
- Travel
- Hospitality
- Financial-Services
---
