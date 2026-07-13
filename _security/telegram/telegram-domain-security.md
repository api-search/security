---
api_specs:
- filename: telegram-bot-openapi.yml
  format: yaml
  label: Telegram Bot API
  slug: telegram-bot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telegram/refs/heads/main/openapi/telegram-bot-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: telegram.org
  spf: true
hosts:
- cert_expires: Sep 12 13:36:48 2026 GMT
  host: core.telegram.org
  hsts: true
  hsts_max_age: 35768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Telegram Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Telegram, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Telegram
provider_slug: telegram
slug: telegram-domain-security
source_filename: telegram-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: core.telegram.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 13:36:48 2026 GMT\n  hsts: true\n  hsts_max_age: 35768000\ndomains:\n- domain: telegram.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telegram/refs/heads/main/security/telegram-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bots
- Chat
- Messaging
- Notifications
- Payments
- Telegram
---
