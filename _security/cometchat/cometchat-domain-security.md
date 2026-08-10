---
api_specs:
- filename: cometchat-auth-tokens-api-openapi.yml
  format: yaml
  label: CometChat Auth Tokens API
  slug: cometchat-auth-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-auth-tokens-api-openapi.yml
- filename: cometchat-banned-users-api-openapi.yml
  format: yaml
  label: CometChat Banned Users API
  slug: cometchat-banned-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-banned-users-api-openapi.yml
- filename: cometchat-blocked-users-api-openapi.yml
  format: yaml
  label: CometChat Blocked Users API
  slug: cometchat-blocked-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-blocked-users-api-openapi.yml
- filename: cometchat-conversations-api-openapi.yml
  format: yaml
  label: CometChat Conversations API
  slug: cometchat-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-conversations-api-openapi.yml
- filename: cometchat-friends-api-openapi.yml
  format: yaml
  label: CometChat Friends API
  slug: cometchat-friends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-friends-api-openapi.yml
- filename: cometchat-group-members-api-openapi.yml
  format: yaml
  label: CometChat Group Members API
  slug: cometchat-group-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-group-members-api-openapi.yml
- filename: cometchat-groups-api-openapi.yml
  format: yaml
  label: CometChat Groups API
  slug: cometchat-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-groups-api-openapi.yml
- filename: cometchat-messages-api-openapi.yml
  format: yaml
  label: CometChat Messages API
  slug: cometchat-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-messages-api-openapi.yml
- filename: cometchat-reactions-api-openapi.yml
  format: yaml
  label: CometChat Reactions API
  slug: cometchat-reactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-reactions-api-openapi.yml
- filename: cometchat-roles-api-openapi.yml
  format: yaml
  label: CometChat Roles API
  slug: cometchat-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-roles-api-openapi.yml
- filename: cometchat-users-api-openapi.yml
  format: yaml
  label: CometChat Users API
  slug: cometchat-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-users-api-openapi.yml
- filename: cometchat-webhooks-api-openapi.yml
  format: yaml
  label: CometChat Webhooks API
  slug: cometchat-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cometchat.com
  spf: true
hosts:
- cert_expires: Sep 17 06:15:44 2026 GMT
  host: www.cometchat.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cometchat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CometChat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CometChat
provider_slug: cometchat
slug: cometchat-domain-security
source_filename: cometchat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cometchat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 06:15:44 2026 GMT\n  hsts: false\ndomains:\n- domain: cometchat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/security/cometchat-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Chat
- Messaging
- Voice
- Video
- SDK
- Realtime
---
