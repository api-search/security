---
api_specs:
- filename: ably-platform-api-openapi.yml
  format: yaml
  label: Ably Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-platform-api-openapi.yml
- filename: ably-control-api-openapi.yml
  format: yaml
  label: Ably Control API
  slug: control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-control-api-openapi.yml
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
- Realtime
- WebSockets
- Pub/Sub
- Messaging
- Streaming
- Push Notifications
- Chat
- LiveSync
---
