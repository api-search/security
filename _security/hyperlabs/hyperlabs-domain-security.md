---
api_specs:
- filename: hyperlabs-web-openapi-original.json
  format: json
  label: HYPERLABS Web API
  slug: hyperlabs-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperlabs/refs/heads/main/openapi/hyperlabs-web-openapi-original.json
- filename: hyperlabs-radium-asyncapi.yml
  format: yaml
  label: HYPERLABS Radium gRPC API (TDR11100)
  slug: hyperlabs-radium-grpc-api-tdr11100
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperlabs/refs/heads/main/asyncapi/hyperlabs-radium-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hyperlabs.com
  spf: false
hosts:
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: www.hyperlabs.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hyperlabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HYPERLABS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: HYPERLABS
provider_slug: hyperlabs
slug: hyperlabs-domain-security
source_filename: hyperlabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hyperlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: hyperlabs.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperlabs/refs/heads/main/security/hyperlabs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- signal-integrity
- Test and Measurement
- Electronic Components
- Instrumentation
- time-domain-reflectometry
- high-speed-digital
- Datacom
- Hardware
- gRPC
- Manufacturing
---
