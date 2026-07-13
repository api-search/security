---
api_specs:
- filename: getstream-openapi.yml
  format: yaml
  label: Stream Chat Channels API
  slug: getstream-chat-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-openapi.yml
- filename: getstream-openapi.yml
  format: yaml
  label: Stream Chat Messages API
  slug: getstream-chat-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-openapi.yml
- filename: getstream-openapi.yml
  format: yaml
  label: Stream Chat Members API
  slug: getstream-chat-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-openapi.yml
- filename: getstream-openapi.yml
  format: yaml
  label: Stream Chat Reactions API
  slug: getstream-chat-reactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-openapi.yml
- filename: getstream-openapi.yml
  format: yaml
  label: Stream Chat Threads API
  slug: getstream-chat-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-openapi.yml
- filename: getstream-openapi.yml
  format: yaml
  label: Stream Chat Users API
  slug: getstream-chat-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-openapi.yml
- filename: getstream-openapi.yml
  format: yaml
  label: Stream Chat Devices and Push API
  slug: getstream-chat-devices-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-openapi.yml
- filename: getstream-openapi.yml
  format: yaml
  label: Stream Chat Moderation API
  slug: getstream-chat-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-openapi.yml
- filename: getstream-openapi.yml
  format: yaml
  label: Stream Chat Permissions and Roles API
  slug: getstream-chat-permissions-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-openapi.yml
- filename: getstream-openapi.yml
  format: yaml
  label: Stream Chat Campaigns API
  slug: getstream-chat-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getstream.io
  spf: true
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "godaddy.com"
  - 0 iodef "mailto:security@getstream.io"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: false
  dnssec: false
  domain: stream-io-api.com
  spf: false
hosts:
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: getstream.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: chat.stream-io-api.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: api.stream-io-api.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Getstream Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stream, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stream
provider_slug: getstream
slug: getstream-domain-security
source_filename: getstream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getstream.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: chat.stream-io-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\n- host: api.stream-io-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: getstream.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: stream-io-api.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 iodef \"mailto:security@getstream.io\"\
  \n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/security/getstream-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Chat
- Messaging
- Activity Feeds
- Video
- Audio
- Moderation
- WebSocket
- Real Time
---
