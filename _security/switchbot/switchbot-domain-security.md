---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: switch-bot.com
  spf: true
hosts:
- cert_expires: Dec 28 13:10:31 2026 GMT
  host: switch-bot.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Switchbot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SwitchBot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SwitchBot
provider_slug: switchbot
slug: switchbot-domain-security
source_filename: switchbot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: switch-bot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 13:10:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: switch-bot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/switchbot/security/switchbot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SmartHome
- IoT
- Automation
- Robotics
- ConsumerElectronics
---
