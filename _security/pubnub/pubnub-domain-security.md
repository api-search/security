---
api_specs:
- filename: pubnub-asyncapi.yml
  format: yaml
  label: PubNub REST API
  slug: rest-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/pubnub/refs/heads/main/asyncapi/pubnub-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pubnub.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pndsn.com
  spf: true
hosts:
- cert_expires: Jan  9 19:00:24 2027 GMT
  host: www.pubnub.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: ps.pndsn.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: admin.pubnub.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pubnub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PubNub, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PubNub
provider_slug: pubnub
slug: pubnub-domain-security
source_filename: pubnub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pubnub.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  9 19:00:24 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: ps.pndsn.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: null\n- host: admin.pubnub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pubnub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: pndsn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pubnub/refs/heads/main/security/pubnub-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Realtime
- WebSockets
- Pub/Sub
- IoT
- Messaging
- Chat
- Presence
- Functions
---
