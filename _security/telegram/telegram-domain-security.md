---
api_specs:
- filename: telegram-bot-info-api-openapi.yml
  format: yaml
  label: Telegram Bot Info API
  slug: telegram-bot-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telegram/refs/heads/main/openapi/telegram-bot-info-api-openapi.yml
- filename: telegram-chat-management-api-openapi.yml
  format: yaml
  label: Telegram Chat Management API
  slug: telegram-chat-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telegram/refs/heads/main/openapi/telegram-chat-management-api-openapi.yml
- filename: telegram-getting-updates-api-openapi.yml
  format: yaml
  label: Telegram Getting Updates API
  slug: telegram-getting-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telegram/refs/heads/main/openapi/telegram-getting-updates-api-openapi.yml
- filename: telegram-invites-api-openapi.yml
  format: yaml
  label: Telegram Invites API
  slug: telegram-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telegram/refs/heads/main/openapi/telegram-invites-api-openapi.yml
- filename: telegram-member-management-api-openapi.yml
  format: yaml
  label: Telegram Member Management API
  slug: telegram-member-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telegram/refs/heads/main/openapi/telegram-member-management-api-openapi.yml
- filename: telegram-message-editing-api-openapi.yml
  format: yaml
  label: Telegram Message Editing API
  slug: telegram-message-editing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telegram/refs/heads/main/openapi/telegram-message-editing-api-openapi.yml
- filename: telegram-messaging-api-openapi.yml
  format: yaml
  label: Telegram Messaging API
  slug: telegram-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telegram/refs/heads/main/openapi/telegram-messaging-api-openapi.yml
- filename: telegram-payments-api-openapi.yml
  format: yaml
  label: Telegram Payments API
  slug: telegram-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telegram/refs/heads/main/openapi/telegram-payments-api-openapi.yml
- filename: telegram-stickers-api-openapi.yml
  format: yaml
  label: Telegram Stickers API
  slug: telegram-stickers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telegram/refs/heads/main/openapi/telegram-stickers-api-openapi.yml
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
- Notification
- Payments
- Telegram
---
