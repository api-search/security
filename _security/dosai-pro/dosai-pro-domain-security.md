---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dosai.pro
  spf: true
hosts:
- cert_expires: Jan 10 01:42:09 2027 GMT
  host: dosai.pro
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DOS AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DOS AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DOS AI
provider_slug: dosai-pro
slug: dosai-pro-domain-security
source_filename: dosai-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dosai.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 01:42:09 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dosai.pro\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dosai-pro/security/dosai-pro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Messaging
- Chatbots
- No-Code
- CRM
- Company
---
