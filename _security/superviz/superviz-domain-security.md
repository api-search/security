---
api_specs:
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Participants API
  slug: superviz-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Channels API
  slug: superviz-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Realtime Data API
  slug: superviz-realtime-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Rooms API
  slug: superviz-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Contextual Comments API
  slug: superviz-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Meetings API
  slug: superviz-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Webhooks API
  slug: superviz-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Authentication API
  slug: superviz-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: superviz.com
  spf: false
hosts:
- cert_expires: Sep 16 14:01:34 2026 GMT
  host: docs.superviz.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: api.superviz.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Superviz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SuperViz, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: SuperViz
provider_slug: superviz
slug: superviz-domain-security
source_filename: superviz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.superviz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 14:01:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.superviz.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: superviz.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/security/superviz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Time
- Collaboration
- Presence
- Synchronization
- Video
- WebRTC
- SDK
---
