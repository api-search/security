---
api_specs:
- filename: getstream-application-api-openapi.yml
  format: yaml
  label: Stream Application API
  slug: getstream-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-application-api-openapi.yml
- filename: getstream-campaigns-api-openapi.yml
  format: yaml
  label: Stream Campaigns API
  slug: getstream-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-campaigns-api-openapi.yml
- filename: getstream-channels-api-openapi.yml
  format: yaml
  label: Stream Channels API
  slug: getstream-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-channels-api-openapi.yml
- filename: getstream-devices-api-openapi.yml
  format: yaml
  label: Stream Devices API
  slug: getstream-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-devices-api-openapi.yml
- filename: getstream-members-api-openapi.yml
  format: yaml
  label: Stream Members API
  slug: getstream-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-members-api-openapi.yml
- filename: getstream-messages-api-openapi.yml
  format: yaml
  label: Stream Messages API
  slug: getstream-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-messages-api-openapi.yml
- filename: getstream-moderation-api-openapi.yml
  format: yaml
  label: Stream Moderation API
  slug: getstream-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-moderation-api-openapi.yml
- filename: getstream-permissions-api-openapi.yml
  format: yaml
  label: Stream Permissions API
  slug: getstream-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-permissions-api-openapi.yml
- filename: getstream-reactions-api-openapi.yml
  format: yaml
  label: Stream Reactions API
  slug: getstream-reactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-reactions-api-openapi.yml
- filename: getstream-roles-api-openapi.yml
  format: yaml
  label: Stream Roles API
  slug: getstream-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-roles-api-openapi.yml
- filename: getstream-threads-api-openapi.yml
  format: yaml
  label: Stream Threads API
  slug: getstream-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-threads-api-openapi.yml
- filename: getstream-users-api-openapi.yml
  format: yaml
  label: Stream Users API
  slug: getstream-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getstream/refs/heads/main/openapi/getstream-users-api-openapi.yml
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
- Real-Time
---
