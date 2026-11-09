---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cutgpt.app
  spf: true
hosts:
- cert_expires: Jan 12 00:25:01 2027 GMT
  host: cutgpt.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cutgpt App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for cutGPT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: cutGPT
provider_slug: cutgpt-app
slug: cutgpt-app-domain-security
source_filename: cutgpt-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cutgpt.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 00:25:01 2027 GMT\n  hsts: false\ndomains:\n- domain: cutgpt.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cutgpt-app/security/cutgpt-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Chat
- Free AI
- Advertising‑funded
- Rewards program
- Mobile App
- PayPal payouts
- ChatGPT alternative
---
