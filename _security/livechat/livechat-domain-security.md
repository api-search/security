---
api_specs:
- filename: livechat-openapi.yml
  format: yaml
  label: LiveChat Agent Chat API
  slug: agent-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livechat/refs/heads/main/openapi/livechat-openapi.yml
- filename: livechat-asyncapi.yml
  format: yaml
  label: LiveChat Webhooks and RTM API
  slug: webhooks-and-rtm
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/livechat/refs/heads/main/openapi/livechat-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: livechat.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: text.com
  spf: true
hosts:
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: www.livechat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: platform.text.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: api.livechatinc.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Livechat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LiveChat, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LiveChat
provider_slug: livechat
slug: livechat-domain-security
source_filename: livechat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.livechat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.text.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.livechatinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: livechat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: text.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/livechat/refs/heads/main/security/livechat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Live Chat
- Customer Service
- Customer Support
- Messaging
- Sales
- Help Desk
---
