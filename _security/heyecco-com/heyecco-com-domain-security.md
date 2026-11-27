---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: heyecco.com
  spf: false
hosts:
- cert_expires: Feb  3 02:36:57 2027 GMT
  host: heyecco.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hey Ecco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hey Ecco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Hey Ecco
provider_slug: heyecco-com
slug: heyecco-com-domain-security
source_filename: heyecco-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heyecco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 02:36:57 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: heyecco.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/heyecco-com/security/heyecco-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Artificial Intelligence
- Productivity
- Boards
- Software-as-a-Service
- Company
---
