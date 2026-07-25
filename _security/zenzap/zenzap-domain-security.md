---
api_specs:
- filename: zenzap-agentic-api-openapi.yml
  format: yaml
  label: ZenZap Agentic API
  slug: zenzap-agentic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenzap/refs/heads/main/openapi/zenzap-agentic-api-openapi.yml
- filename: zenzap-long-polling-api-openapi.yml
  format: yaml
  label: ZenZap Long Polling API
  slug: zenzap-long-polling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenzap/refs/heads/main/openapi/zenzap-long-polling-api-openapi.yml
- filename: zenzap-members-api-openapi.yml
  format: yaml
  label: ZenZap Members API
  slug: zenzap-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenzap/refs/heads/main/openapi/zenzap-members-api-openapi.yml
- filename: zenzap-messages-api-openapi.yml
  format: yaml
  label: ZenZap Messages API
  slug: zenzap-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenzap/refs/heads/main/openapi/zenzap-messages-api-openapi.yml
- filename: zenzap-oauth-api-openapi.yml
  format: yaml
  label: ZenZap OAuth API
  slug: zenzap-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenzap/refs/heads/main/openapi/zenzap-oauth-api-openapi.yml
- filename: zenzap-polls-api-openapi.yml
  format: yaml
  label: ZenZap Polls API
  slug: zenzap-polls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenzap/refs/heads/main/openapi/zenzap-polls-api-openapi.yml
- filename: zenzap-tasks-api-openapi.yml
  format: yaml
  label: ZenZap Tasks API
  slug: zenzap-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenzap/refs/heads/main/openapi/zenzap-tasks-api-openapi.yml
- filename: zenzap-topics-group-chats-channels-conversations-api-openapi.yml
  format: yaml
  label: ZenZap Topics (group chats/channels/conversations) API
  slug: zenzap-topics-group-chats-channels-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenzap/refs/heads/main/openapi/zenzap-topics-group-chats-channels-conversations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zenzap.co
  spf: true
hosts:
- cert_expires: Oct  1 07:45:12 2026 GMT
  host: www.zenzap.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 01:21:33 2026 GMT
  host: api.zenzap.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zenzap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZenZap, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ZenZap
provider_slug: zenzap
slug: zenzap-domain-security
source_filename: zenzap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zenzap.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 07:45:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.zenzap.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 01:21:33 2026 GMT\n  hsts: null\ndomains:\n- domain: zenzap.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenzap/refs/heads/main/security/zenzap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Messaging
- Team Communication
- Collaboration
- Chat
- Bots
- Webhooks
- Productivity
- Tasks
---
