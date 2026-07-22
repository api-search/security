---
api_specs:
- filename: rainway-hub-api-openapi.yml
  format: yaml
  label: Rainway Hub API
  slug: rainway-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainway/refs/heads/main/openapi/rainway-hub-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: rainway.com
  spf: true
hosts:
- cert_expires: Sep  4 17:45:55 2026 GMT
  host: rainway.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 17:45:55 2026 GMT
  host: hub-api.rainway.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rainway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rainway, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Rainway
provider_slug: rainway
slug: rainway-domain-security
source_filename: rainway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rainway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 17:45:55 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: hub-api.rainway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 17:45:55 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: rainway.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rainway/refs/heads/main/security/rainway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Streaming
- Application Streaming
- WebRTC
- Game Streaming
- SDK
- Real-Time
- Developer Platform
---
