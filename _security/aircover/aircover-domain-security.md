---
api_specs:
- filename: aircover-openapi.yml
  format: yaml
  label: Aircover Public Agent API
  slug: aircover-public-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aircover/refs/heads/main/openapi/aircover-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aircover.ai
  spf: true
hosts:
- cert_expires: Dec 10 23:28:53 2026 GMT
  host: www.aircover.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 03:38:31 2026 GMT
  host: api.aircover.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Aircover Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aircover, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aircover
provider_slug: aircover
slug: aircover-domain-security
source_filename: aircover-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aircover.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:28:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.aircover.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 03:38:31 2026 GMT\n  hsts: null\ndomains:\n- domain: aircover.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aircover/refs/heads/main/security/aircover-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales Enablement
- Conversation Intelligence
- Sales Coaching
- Revenue Intelligence
- AI Agents
- MCP
- agent-native
- CRM
- Meetings
- Transcription
- Authentication
---
