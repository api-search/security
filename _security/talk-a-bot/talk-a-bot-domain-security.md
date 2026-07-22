---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: talkabot.net
  spf: true
hosts:
- cert_expires: Oct  2 18:19:29 2026 GMT
  host: talkabot.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Talk A Bot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Talk-A-Bot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Talk-A-Bot
provider_slug: talk-a-bot
slug: talk-a-bot-domain-security
source_filename: talk-a-bot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: talkabot.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:19:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: talkabot.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talk-a-bot/refs/heads/main/security/talk-a-bot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Chatbots
- Conversational AI
- Enterprise Software
- Compliance
- Customer Support
- Artificial Intelligence
---
