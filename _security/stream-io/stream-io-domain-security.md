---
api_specs:
- filename: stream-io-chat-openapi.yml
  format: yaml
  label: Stream Chat API
  slug: chat
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stream-io/refs/heads/main/openapi/stream-io-chat-openapi.yml
- filename: stream-io-video-openapi.yml
  format: yaml
  label: Stream Video & Audio API
  slug: video
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stream-io/refs/heads/main/openapi/stream-io-video-openapi.yml
- filename: stream-io-moderation-openapi.yml
  format: yaml
  label: Stream Moderation API
  slug: moderation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stream-io/refs/heads/main/openapi/stream-io-moderation-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:security@getstream.io"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getstream.io
  spf: true
- caa:
  - 0 issue "godaddy.com"
  - 0 iodef "mailto:security@getstream.io"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
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
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: video.stream-io-api.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stream Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stream, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stream
provider_slug: stream-io
slug: stream-io-domain-security
source_filename: stream-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getstream.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: chat.stream-io-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\n- host: video.stream-io-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: getstream.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:security@getstream.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: stream-io-api.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 iodef \"mailto:security@getstream.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue\
  \ \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stream-io/refs/heads/main/security/stream-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Realtime
- Chat
- Messaging
- Video
- Audio
- Activity Feeds
- Moderation
- SDK
---
