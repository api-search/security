---
api_specs:
- filename: demodesk-v2-openapi.yml
  format: yaml
  label: Demodesk Public API (v2)
  slug: demodesk-public-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demodesk/refs/heads/main/openapi/demodesk-v2-openapi.yml
- filename: demodesk-v1-openapi.json
  format: json
  label: Demodesk API V1 (deprecated)
  slug: demodesk-api-v1-deprecated
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demodesk/refs/heads/main/openapi/demodesk-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: demodesk.com
  spf: true
hosts:
- cert_expires: Sep 11 19:04:40 2026 GMT
  host: demodesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Demodesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Demodesk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Demodesk
provider_slug: demodesk
slug: demodesk-domain-security
source_filename: demodesk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: demodesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 19:04:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: demodesk.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demodesk/refs/heads/main/security/demodesk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Sales
- AI
- Conversation Intelligence
- Video Conferencing
- CRM
- Transcription
- Webhooks
- MCP
---
