---
api_specs:
- filename: cometchat-openapi.yml
  format: yaml
  label: CometChat Users API
  slug: cometchat-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-openapi.yml
- filename: cometchat-openapi.yml
  format: yaml
  label: CometChat Groups & Members API
  slug: cometchat-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-openapi.yml
- filename: cometchat-openapi.yml
  format: yaml
  label: CometChat Messages API
  slug: cometchat-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-openapi.yml
- filename: cometchat-openapi.yml
  format: yaml
  label: CometChat Conversations API
  slug: cometchat-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-openapi.yml
- filename: cometchat-openapi.yml
  format: yaml
  label: CometChat Roles API
  slug: cometchat-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-openapi.yml
- filename: cometchat-openapi.yml
  format: yaml
  label: CometChat Relationships API
  slug: cometchat-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-openapi.yml
- filename: cometchat-openapi.yml
  format: yaml
  label: CometChat Webhooks API
  slug: cometchat-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/openapi/cometchat-openapi.yml
- filename: cometchat-asyncapi.yml
  format: yaml
  label: CometChat Realtime & Client SDK
  slug: cometchat-realtime-sdk
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cometchat/refs/heads/main/asyncapi/cometchat-asyncapi.yml
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
