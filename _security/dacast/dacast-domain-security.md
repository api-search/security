---
api_specs:
- filename: dacast-openapi.yml
  format: yaml
  label: Dacast VOD API
  slug: dacast-vod-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dacast/refs/heads/main/openapi/dacast-openapi.yml
- filename: dacast-openapi.yml
  format: yaml
  label: Dacast Live Channels API
  slug: dacast-live-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dacast/refs/heads/main/openapi/dacast-openapi.yml
- filename: dacast-openapi.yml
  format: yaml
  label: Dacast Playlists API
  slug: dacast-playlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dacast/refs/heads/main/openapi/dacast-openapi.yml
- filename: dacast-openapi.yml
  format: yaml
  label: Dacast Analytics API
  slug: dacast-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dacast/refs/heads/main/openapi/dacast-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "geotrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dacast.com
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: www.dacast.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 11:29:58 2026 GMT
  host: docs.dacast.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: developer.dacast.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dacast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dacast, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dacast
provider_slug: dacast
slug: dacast-domain-security
source_filename: dacast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dacast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\n- host: docs.dacast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 11:29:58 2026 GMT\n  hsts: null\n- host: developer.dacast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: dacast.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"geotrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dacast/refs/heads/main/security/dacast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Live Streaming
- Video
- VOD
- OTT
- Video Hosting
- Media
- Analytics
---
