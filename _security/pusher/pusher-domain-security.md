---
api_specs:
- filename: pusher-asyncapi.yml
  format: yaml
  label: Pusher Channels API
  slug: channels-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/pusher/refs/heads/main/asyncapi/pusher-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pusher.com
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: pusher.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pusher Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pusher, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pusher
provider_slug: pusher
slug: pusher-domain-security
source_filename: pusher-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pusher.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pusher.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pusher/refs/heads/main/security/pusher-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Realtime
- WebSockets
- Pub/Sub
- Push Notifications
- Messaging
---
