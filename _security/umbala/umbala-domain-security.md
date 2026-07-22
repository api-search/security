---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: umbala.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: umbala.tv
  spf: false
hosts:
- cert_expires: Sep  7 05:24:14 2026 GMT
  host: umbala.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 15:58:15 2026 GMT
  host: umbala.tv
  hsts: true
  hsts_max_age: 31536000
  https: true
  repurposed: redirects to unrelated gambling site (barrybulakites.co)
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Umbala Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Umbala, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Umbala
provider_slug: umbala
slug: umbala-domain-security
source_filename: umbala-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  umbala.io is the company's current site (Umbala Labs). The historical\n  product domain umbala.tv no longer serves company content — it\n  301-redirects via 789bets.biz to barrybulakites.co, an unrelated\n  gambling site — but its posture is recorded since it remains associated\n  with the brand.\nhosts:\n- host: umbala.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 05:24:14 2026 GMT\n  hsts: false\n- host: umbala.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 15:58:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  repurposed: redirects to unrelated gambling site (barrybulakites.co)\ndomains:\n- domain: umbala.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: umbala.tv\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/umbala/refs/heads/main/security/umbala-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Video
- Streaming
- Camera
- Blockchain
- Mobile
---
