---
api_specs:
- filename: lvt-cameras-api-openapi.yml
  format: yaml
  label: LVT Cameras API
  slug: lvt-cameras-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-cameras-api-openapi.yml
- filename: lvt-events-api-openapi.yml
  format: yaml
  label: LVT Events API
  slug: lvt-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-events-api-openapi.yml
- filename: lvt-liveunits-api-openapi.yml
  format: yaml
  label: LVT Live Units API
  slug: lvt-liveunits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-liveunits-api-openapi.yml
- filename: lvt-locations-api-openapi.yml
  format: yaml
  label: LVT Locations API
  slug: lvt-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-locations-api-openapi.yml
- filename: lvt-media-api-openapi.yml
  format: yaml
  label: LVT Media API
  slug: lvt-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-media-api-openapi.yml
- filename: lvt-publickeys-api-openapi.yml
  format: yaml
  label: LVT Public Keys API
  slug: lvt-publickeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-publickeys-api-openapi.yml
- filename: lvt-streams-api-openapi.yml
  format: yaml
  label: LVT Streams API
  slug: lvt-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-streams-api-openapi.yml
- filename: lvt-talkdown-api-openapi.yml
  format: yaml
  label: LVT Talkdown API
  slug: lvt-talkdown-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-talkdown-api-openapi.yml
- filename: lvt-webhooks-api-openapi.yml
  format: yaml
  label: LVT Webhooks API
  slug: lvt-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/openapi/lvt-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lvt.com
  spf: true
hosts:
- cert_expires: Nov 23 04:16:20 2026 GMT
  host: www.lvt.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 16:02:24 2026 GMT
  host: docs.lvt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: api.lvt.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Lvt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LVT, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LVT
provider_slug: lvt
slug: lvt-domain-security
source_filename: lvt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lvt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 04:16:20 2026 GMT\n  hsts: false\n- host: docs.lvt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 16:02:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lvt.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: lvt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lvt/refs/heads/main/security/lvt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Physical Security
- Video Surveillance
- Camera
- Video Streaming
- WebRTC
- RTSP
- ONVIF
- IoT
- Alerts
- Webhook
- Public Safety
- Retail
- Critical Infrastructure
---
