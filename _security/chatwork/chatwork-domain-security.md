---
api_specs:
- filename: chatwork-contacts-api-openapi.yml
  format: yaml
  label: Chatwork Contacts API
  slug: chatwork-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwork/refs/heads/main/openapi/chatwork-contacts-api-openapi.yml
- filename: chatwork-files-api-openapi.yml
  format: yaml
  label: Chatwork Files API
  slug: chatwork-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwork/refs/heads/main/openapi/chatwork-files-api-openapi.yml
- filename: chatwork-incoming-requests-api-openapi.yml
  format: yaml
  label: Chatwork Incoming Requests API
  slug: chatwork-incoming-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwork/refs/heads/main/openapi/chatwork-incoming-requests-api-openapi.yml
- filename: chatwork-link-api-openapi.yml
  format: yaml
  label: Chatwork Link API
  slug: chatwork-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwork/refs/heads/main/openapi/chatwork-link-api-openapi.yml
- filename: chatwork-me-api-openapi.yml
  format: yaml
  label: Chatwork Me API
  slug: chatwork-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwork/refs/heads/main/openapi/chatwork-me-api-openapi.yml
- filename: chatwork-members-api-openapi.yml
  format: yaml
  label: Chatwork Members API
  slug: chatwork-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwork/refs/heads/main/openapi/chatwork-members-api-openapi.yml
- filename: chatwork-messages-api-openapi.yml
  format: yaml
  label: Chatwork Messages API
  slug: chatwork-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwork/refs/heads/main/openapi/chatwork-messages-api-openapi.yml
- filename: chatwork-rooms-api-openapi.yml
  format: yaml
  label: Chatwork Rooms API
  slug: chatwork-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwork/refs/heads/main/openapi/chatwork-rooms-api-openapi.yml
- filename: chatwork-tasks-api-openapi.yml
  format: yaml
  label: Chatwork Tasks API
  slug: chatwork-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatwork/refs/heads/main/openapi/chatwork-tasks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chatwork.com
  spf: true
hosts:
- cert_expires: Jul 27 09:03:03 2026 GMT
  host: go.chatwork.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  4 06:00:43 2026 GMT
  host: developer.chatwork.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: api.chatwork.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chatwork Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chatwork, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chatwork
provider_slug: chatwork
slug: chatwork-domain-security
source_filename: chatwork-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: go.chatwork.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 27 09:03:03 2026 GMT\n  hsts: false\n- host: developer.chatwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 06:00:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.chatwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: chatwork.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chatwork/refs/heads/main/security/chatwork-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Messaging
- Chat
- Collaboration
- Productivity
- Task
---
