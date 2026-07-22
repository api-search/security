---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mybots.pro
  spf: true
hosts:
- cert_expires: Sep  9 06:36:56 2026 GMT
  host: mybots.pro
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mybotspro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mybots.pro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Mybots.pro
provider_slug: mybotspro
slug: mybotspro-domain-security
source_filename: mybotspro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mybots.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 06:36:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mybots.pro\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mybotspro/refs/heads/main/security/mybotspro-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI Agents
- Conversational AI
- Messaging
- Chatbots
- Customer Support
- Sales Automation
- WhatsApp
- Telegram
---
