---
api_specs:
- filename: ably-apps-api-openapi.yml
  format: yaml
  label: Ably apps API
  slug: ably-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-apps-api-openapi.yml
- filename: ably-authentication-api-openapi.yml
  format: yaml
  label: Ably Authentication API
  slug: ably-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-authentication-api-openapi.yml
- filename: ably-history-api-openapi.yml
  format: yaml
  label: Ably History API
  slug: ably-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-history-api-openapi.yml
- filename: ably-keys-api-openapi.yml
  format: yaml
  label: Ably keys API
  slug: ably-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-keys-api-openapi.yml
- filename: ably-namespaces-api-openapi.yml
  format: yaml
  label: Ably namespaces API
  slug: ably-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-namespaces-api-openapi.yml
- filename: ably-publishing-api-openapi.yml
  format: yaml
  label: Ably Publishing API
  slug: ably-publishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-publishing-api-openapi.yml
- filename: ably-push-api-openapi.yml
  format: yaml
  label: Ably Push API
  slug: ably-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-push-api-openapi.yml
- filename: ably-queues-api-openapi.yml
  format: yaml
  label: Ably queues API
  slug: ably-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-queues-api-openapi.yml
- filename: ably-rules-api-openapi.yml
  format: yaml
  label: Ably rules API
  slug: ably-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-rules-api-openapi.yml
- filename: ably-stats-api-openapi.yml
  format: yaml
  label: Ably Stats API
  slug: ably-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-stats-api-openapi.yml
- filename: ably-status-api-openapi.yml
  format: yaml
  label: Ably Status API
  slug: ably-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-status-api-openapi.yml
- filename: ably-tokens-api-openapi.yml
  format: yaml
  label: Ably tokens API
  slug: ably-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-tokens-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ably.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ably.io
  spf: true
hosts:
- cert_expires: Sep 12 01:41:22 2026 GMT
  host: ably.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: rest.ably.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: control.ably.net
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ably Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ably, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ably
provider_slug: ably
slug: ably-domain-security
source_filename: ably-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ably.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 01:41:22 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: rest.ably.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\n- host: control.ably.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ably.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ably.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/security/ably-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Real-Time
- WebSockets
- Pub-Sub
- Messaging
- Streaming
- Push Notifications
- Chat
- LiveSync
---
