---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: answer.ai
  spf: true
hosts:
- cert_expires: Jan  2 21:48:20 2027 GMT
  host: answer.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Answerai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Answer.AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Answer.AI
provider_slug: answerai
slug: answerai-domain-security
source_filename: answerai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: answer.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 21:48:20 2027 GMT\n  hsts: false\ndomains:\n- domain: answer.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/answerai/security/answerai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Research
- OpenSource
- Products
---
