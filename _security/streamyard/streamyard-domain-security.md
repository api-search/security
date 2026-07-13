---
api_specs:
- filename: streamyard-openapi.yml
  format: yaml
  label: StreamYard API
  slug: streamyard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamyard/refs/heads/main/openapi/streamyard-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: streamyard.com
  spf: true
hosts:
- cert_expires: Sep  5 15:19:14 2026 GMT
  host: streamyard.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 15:19:14 2026 GMT
  host: developers.streamyard.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 15:19:14 2026 GMT
  host: api.streamyard.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Streamyard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StreamYard, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: StreamYard
provider_slug: streamyard
slug: streamyard-domain-security
source_filename: streamyard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: streamyard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 15:19:14 2026 GMT\n  hsts: false\n- host: developers.streamyard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 15:19:14 2026 GMT\n  hsts: false\n- host: api.streamyard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 15:19:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: streamyard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/streamyard/refs/heads/main/security/streamyard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Broadcasting
- Live Streaming
- Multi-Streaming
- Recordings
- Video
---
