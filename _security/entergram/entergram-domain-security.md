---
api_specs:
- filename: entergram-accounts-api-openapi.yml
  format: yaml
  label: Entergram Accounts API
  slug: entergram-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-accounts-api-openapi.yml
- filename: entergram-chat-commands-api-openapi.yml
  format: yaml
  label: Entergram Chat Commands API
  slug: entergram-chat-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-chat-commands-api-openapi.yml
- filename: entergram-chats-api-openapi.yml
  format: yaml
  label: Entergram Chats API
  slug: entergram-chats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-chats-api-openapi.yml
- filename: entergram-contacts-api-openapi.yml
  format: yaml
  label: Entergram Contacts API
  slug: entergram-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-contacts-api-openapi.yml
- filename: entergram-custom-fields-api-openapi.yml
  format: yaml
  label: Entergram Custom Fields API
  slug: entergram-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-custom-fields-api-openapi.yml
- filename: entergram-events-api-openapi.yml
  format: yaml
  label: Entergram Events API
  slug: entergram-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-events-api-openapi.yml
- filename: entergram-groups-api-openapi.yml
  format: yaml
  label: Entergram Groups API
  slug: entergram-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-groups-api-openapi.yml
- filename: entergram-live-chats-api-openapi.yml
  format: yaml
  label: Entergram Live Chats API
  slug: entergram-live-chats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-live-chats-api-openapi.yml
- filename: entergram-make-webhooks-api-openapi.yml
  format: yaml
  label: Entergram Make webhooks API
  slug: entergram-make-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-make-webhooks-api-openapi.yml
- filename: entergram-members-api-openapi.yml
  format: yaml
  label: Entergram Members API
  slug: entergram-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-members-api-openapi.yml
- filename: entergram-messages-api-openapi.yml
  format: yaml
  label: Entergram Messages API
  slug: entergram-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-messages-api-openapi.yml
- filename: entergram-system-api-openapi.yml
  format: yaml
  label: Entergram System API
  slug: entergram-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-system-api-openapi.yml
- filename: entergram-tickets-api-openapi.yml
  format: yaml
  label: Entergram Tickets API
  slug: entergram-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-tickets-api-openapi.yml
- filename: entergram-webhooks-api-openapi.yml
  format: yaml
  label: Entergram Webhooks API
  slug: entergram-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-webhooks-api-openapi.yml
- filename: entergram-workspace-api-openapi.yml
  format: yaml
  label: Entergram Workspace API
  slug: entergram-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-workspace-api-openapi.yml
- filename: entergram-workspace-chats-api-openapi.yml
  format: yaml
  label: Entergram Workspace Chats API
  slug: entergram-workspace-chats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-workspace-chats-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: entergram.com
  spf: true
hosts:
- cert_expires: Nov  2 15:17:44 2026 GMT
  host: api.entergram.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Entergram Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Entergram, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Entergram
provider_slug: entergram
slug: entergram-domain-security
source_filename: entergram-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.entergram.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 15:17:44 2026 GMT\n  hsts: null\ndomains:\n- domain: entergram.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/security/entergram-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Messaging
- Notification
- Communications
- CRM
- Telegram
- Customer-Support
- Ticketing
- Sales
- MCP
- Webhook
---
