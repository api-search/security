---
api_specs:
- filename: api-video-openapi.yml
  format: yaml
  label: api.video Video On Demand API
  slug: video-on-demand
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-video/refs/heads/main/openapi/api-video-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: api.video
  spf: true
hosts:
- cert_expires: Sep 18 11:40:22 2026 GMT
  host: api.video
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 11:23:30 2026 GMT
  host: docs.api.video
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 23:59:59 2026 GMT
  host: ws.api.video
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Api Video Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for API.Video, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: API.Video
provider_slug: api-video
slug: api-video-domain-security
source_filename: api-video-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.video\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 11:40:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.api.video\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 11:23:30 2026 GMT\n  hsts: false\n- host: ws.api.video\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: api.video\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-video/refs/heads/main/security/api-video-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Analytics
- CDN
- Encoding
- Live Streaming
- Transcription
- Video
- Video on Demand
---
