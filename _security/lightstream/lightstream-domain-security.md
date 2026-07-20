---
api_specs:
- filename: lightstream-live-openapi-original.yml
  format: yaml
  label: API.stream Live API
  slug: live-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightstream/refs/heads/main/openapi/lightstream-live-openapi-original.yml
- filename: lightstream-layout-openapi-original.yml
  format: yaml
  label: API.stream Layout API
  slug: layout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightstream/refs/heads/main/openapi/lightstream-layout-openapi-original.yml
- filename: lightstream-event-openapi-original.yml
  format: yaml
  label: API.stream Event API
  slug: event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightstream/refs/heads/main/openapi/lightstream-event-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: golightstream.com
  spf: true
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: api.stream
  spf: true
hosts:
- cert_expires: Sep 19 15:01:14 2026 GMT
  host: golightstream.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 11:02:10 2026 GMT
  host: www.api.stream
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 11:02:10 2026 GMT
  host: live.api.stream
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lightstream Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lightstream, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lightstream
provider_slug: lightstream
slug: lightstream-domain-security
source_filename: lightstream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: golightstream.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:01:14 2026 GMT\n  hsts: false\n- host: www.api.stream\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 11:02:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: live.api.stream\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 11:02:10 2026 GMT\n  hsts: null\ndomains:\n- domain: golightstream.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: api.stream\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightstream/refs/heads/main/security/lightstream-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Video
- Live Streaming
- Broadcasting
- WebRTC
- RTMP
- Media
- Compositing
- Real Time
- Events
- gRPC
- Creator Tools
---
