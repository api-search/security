---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: com.bot
  spf: true
hosts:
- cert_expires: Jan  8 09:49:45 2027 GMT
  host: com.bot
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Com Bot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for com-bot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: com-bot
provider_slug: com-bot
slug: com-bot-domain-security
source_filename: com-bot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: com.bot\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 09:49:45 2027 GMT\n  hsts: false\ndomains:\n- domain: com.bot\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/com-bot/security/com-bot-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Messaging
- Automation
- WhatsApp
- SaaS
- India
---
