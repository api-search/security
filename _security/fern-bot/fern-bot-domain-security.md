---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: fern.bot
  spf: false
hosts:
- cert_expires: Sep 13 03:05:59 2026 GMT
  host: fern.bot
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fern Bot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fern Bot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Fern Bot
provider_slug: fern-bot
slug: fern-bot-domain-security
source_filename: fern-bot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fern.bot\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 03:05:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fern.bot\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fern-bot/refs/heads/main/security/fern-bot-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Robotics
- Physical AI
- Reinforcement Learning
- World Models
- Simulation
- Infrastructure
- Y Combinator
---
