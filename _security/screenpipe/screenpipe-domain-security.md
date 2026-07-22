---
api_specs:
- filename: screenpipe-openapi-original.yml
  format: yaml
  label: Screenpipe Local REST API
  slug: screenpipe-local-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenpipe/refs/heads/main/openapi/screenpipe-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: screenpi.pe
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: screenpipe.com
  spf: false
hosts:
- cert_expires: Oct 13 07:23:35 2026 GMT
  host: screenpi.pe
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 15:09:24 2026 GMT
  host: docs.screenpipe.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Screenpipe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Screenpipe, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Screenpipe
provider_slug: screenpipe
slug: screenpipe-domain-security
source_filename: screenpipe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: screenpi.pe\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 07:23:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.screenpipe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 15:09:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: screenpi.pe\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: screenpipe.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/screenpipe/refs/heads/main/security/screenpipe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Screen Recording
- Screen Memory
- Audio Transcription
- Meeting Intelligence
- Local First
- Privacy
- AI Agents
- MCP
- Developer Tools
- Productivity
- Open Source
---
