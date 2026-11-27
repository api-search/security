---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fitnito.com
  spf: true
hosts:
- cert_expires: Feb  4 04:05:58 2027 GMT
  host: fitnito.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fitnito Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fitnito, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fitnito
provider_slug: fitnito-com
slug: fitnito-com-domain-security
source_filename: fitnito-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fitnito.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 04:05:58 2027 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: fitnito.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fitnito-com/security/fitnito-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Scheduling
- Payments
- Client Management
- Fitness
- AI Assistant
- Small Gyms
---
