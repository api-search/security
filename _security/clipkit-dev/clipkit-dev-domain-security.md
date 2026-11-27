---
api_specs:
- filename: clipkit-dev-openapi-generated.yml
  format: yaml
  label: Clipkit Render API
  slug: clipkit-dev-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipkit-dev/openapi/_ae-authored/clipkit-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clipkit.dev
  spf: true
hosts:
- cert_expires: Dec 31 04:31:04 2026 GMT
  host: clipkit.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clipkit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clipkit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clipkit
provider_slug: clipkit-dev
slug: clipkit-dev-domain-security
source_filename: clipkit-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clipkit.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 04:31:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: clipkit.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/clipkit-dev/security/clipkit-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Video
- Video Rendering
- AI Agents
- MCP
- JSON
- Open Source
- Developer Tools
---
