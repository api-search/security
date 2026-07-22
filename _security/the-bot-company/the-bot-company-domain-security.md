---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bot.co
  spf: true
hosts:
- cert_expires: Sep 13 23:57:57 2026 GMT
  host: www.bot.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Bot Company Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Bot Company, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: The Bot Company
provider_slug: the-bot-company
slug: the-bot-company-domain-security
source_filename: the-bot-company-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bot.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:57:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bot.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-bot-company/refs/heads/main/security/the-bot-company-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Robotics
- Household Robots
- Consumer Robotics
- Automation
- Hardware
- Artificial Intelligence
---
