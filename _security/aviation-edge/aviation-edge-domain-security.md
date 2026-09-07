---
api_specs:
- filename: aviation-edge-openapi.yml
  format: yaml
  label: Aviation Edge
  slug: aviation-edge
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aviation-edge/refs/heads/main/openapi/_original/aviation-edge-openapi.yml
- filename: aviation-edge-real-time-api-openapi.yml
  format: yaml
  label: Aviation Edge Real-Time API
  slug: aviation-edge-real-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aviation-edge/refs/heads/main/openapi/aviation-edge-real-time-api-openapi.yml
- filename: aviation-edge-reference-api-openapi.yml
  format: yaml
  label: Aviation Edge Reference API
  slug: aviation-edge-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aviation-edge/refs/heads/main/openapi/aviation-edge-reference-api-openapi.yml
- filename: aviation-edge-satellites-api-openapi.yml
  format: yaml
  label: Aviation Edge Satellites API
  slug: aviation-edge-satellites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aviation-edge/refs/heads/main/openapi/aviation-edge-satellites-api-openapi.yml
- filename: aviation-edge-schedules-api-openapi.yml
  format: yaml
  label: Aviation Edge Schedules API
  slug: aviation-edge-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aviation-edge/refs/heads/main/openapi/aviation-edge-schedules-api-openapi.yml
- filename: aviation-edge-notams-api-openapi.yml
  format: yaml
  label: Aviation Edge NOTAMs API
  slug: aviation-edge-notams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aviation-edge/refs/heads/main/openapi/aviation-edge-notams-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aviation-edge.com
  spf: true
hosts:
- cert_expires: Nov 10 15:12:56 2026 GMT
  host: aviation-edge.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aviation Edge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aviation Edge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aviation Edge
provider_slug: aviation-edge
slug: aviation-edge-domain-security
source_filename: aviation-edge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aviation-edge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 15:12:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aviation-edge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aviation-edge/refs/heads/main/security/aviation-edge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Airlines
- Airports
- Aviation
- Flight Data
- Real-Time
---
