---
api_specs:
- filename: aircube-openapi-generated.yml
  format: yaml
  label: AirCube API
  slug: aircube-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aircube/refs/heads/main/openapi/_ae-authored/aircube-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aircube.ai
  spf: true
hosts:
- cert_expires: Nov 27 10:54:01 2026 GMT
  host: aircube.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.aircube.ai
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Aircube Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AirCube, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AirCube
provider_slug: aircube
slug: aircube-domain-security
source_filename: aircube-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aircube.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 10:54:01 2026 GMT\n  hsts: false\n- host: api.aircube.ai\n  https: false\ndomains:\n- domain: aircube.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aircube/refs/heads/main/security/aircube-domain-security.yml
summary_line: TLSv1.3
tags:
- AI
- Platform
- API
- MediaGeneration
- UnifiedAPI
---
