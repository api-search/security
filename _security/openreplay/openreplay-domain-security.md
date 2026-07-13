---
api_specs:
- filename: openreplay-openapi.yml
  format: yaml
  label: OpenReplay API
  slug: openreplay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openreplay/refs/heads/main/openapi/openreplay-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openreplay.com
  spf: true
hosts:
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: openreplay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: api.openreplay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openreplay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenReplay, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenReplay
provider_slug: openreplay
slug: openreplay-domain-security
source_filename: openreplay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openreplay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.openreplay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: openreplay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openreplay/refs/heads/main/security/openreplay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Debugging
- Error Tracking
- Open Source
- Performance Monitoring
- Session Replay
- User Behavior
---
