---
api_specs:
- filename: openapi.json
  format: json
  label: SpaceAPI Collector
  slug: spaceapi-collector
  spec_type: OpenAPI
  url: https://api.spaceapi.io/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: spaceapi.io
  spf: false
hosts:
- cert_expires: Aug 12 10:54:23 2026 GMT
  host: spaceapi.io
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.3
- host: collector.spaceapi.io
  https: false
kind: domain-security
layout: security
method: probed
name: Spaceapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpaceAPI, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: SpaceAPI
provider_slug: spaceapi
slug: spaceapi-domain-security
source_filename: spaceapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spaceapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 10:54:23 2026 GMT\n  hsts: true\n  hsts_max_age: 315360000\n- host: collector.spaceapi.io\n  https: false\ndomains:\n- domain: spaceapi.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spaceapi/refs/heads/main/security/spaceapi-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Co-Working
- Event Spaces
- Maker Spaces
- Hackerspaces
- Community
- Open Standard
---
