---
api_specs:
- filename: pushbullet-openapi.yml
  format: yaml
  label: Pushbullet HTTP API
  slug: http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-openapi.yml
- filename: pushbullet-asyncapi.yml
  format: yaml
  label: Pushbullet Realtime Event Stream
  slug: realtime-event-stream
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/openapi/pushbullet-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pushbullet.com
  spf: true
hosts:
- cert_expires: Oct  6 02:39:23 2026 GMT
  host: www.pushbullet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 02:39:23 2026 GMT
  host: docs.pushbullet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 17:50:04 2026 GMT
  host: api.pushbullet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pushbullet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pushbullet, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pushbullet
provider_slug: pushbullet
slug: pushbullet-domain-security
source_filename: pushbullet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pushbullet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 02:39:23 2026 GMT\n  hsts: false\n- host: docs.pushbullet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 02:39:23 2026 GMT\n  hsts: false\n- host: api.pushbullet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 17:50:04 2026 GMT\n  hsts: null\ndomains:\n- domain: pushbullet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pushbullet/refs/heads/main/security/pushbullet-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Notifications
- Messaging
- Push Notifications
- Device Sync
- SMS
- File Transfer
---
