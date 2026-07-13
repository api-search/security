---
api_specs:
- filename: castr-live-openapi.yml
  format: yaml
  label: Castr Live Streams API
  slug: castr-live-live-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castr-live/refs/heads/main/openapi/castr-live-openapi.yml
- filename: castr-live-openapi.yml
  format: yaml
  label: Castr Sub-Second Streams API
  slug: castr-live-sub-second-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castr-live/refs/heads/main/openapi/castr-live-openapi.yml
- filename: castr-live-openapi.yml
  format: yaml
  label: Castr Video Hosting and VOD API
  slug: castr-live-video-hosting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castr-live/refs/heads/main/openapi/castr-live-openapi.yml
- filename: castr-live-openapi.yml
  format: yaml
  label: Castr Analytics and Activity API
  slug: castr-live-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castr-live/refs/heads/main/openapi/castr-live-openapi.yml
- filename: castr-live-openapi.yml
  format: yaml
  label: Castr Webhooks API
  slug: castr-live-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castr-live/refs/heads/main/openapi/castr-live-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: castr.com
  spf: true
hosts:
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: castr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  3 18:31:27 2026 GMT
  host: developers.castr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: api.castr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Castr Live Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Castr, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Castr
provider_slug: castr-live
slug: castr-live-domain-security
source_filename: castr-live-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: castr.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.castr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 18:31:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.castr.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: castr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/castr-live/refs/heads/main/security/castr-live-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Live Streaming
- Multistreaming
- Video Hosting
- VOD
- Video
- Restreaming
- Sub-Second Streaming
- WebRTC
- Analytics
- Webhooks
---
