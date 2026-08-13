---
api_specs:
- filename: flora-fauna-flora-api-openapi.yml
  format: yaml
  label: Flora.ai API
  slug: flora-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flora-fauna/refs/heads/main/openapi/flora-fauna-flora-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: florafauna.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flora.ai
  spf: true
hosts:
- cert_expires: Oct  4 23:54:55 2026 GMT
  host: www.florafauna.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 07:04:14 2026 GMT
  host: developer.flora.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:47:54 2026 GMT
  host: app.flora.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flora Fauna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FLORA, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FLORA
provider_slug: flora-fauna
slug: flora-fauna-domain-security
source_filename: flora-fauna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.florafauna.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:54:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.flora.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 07:04:14 2026 GMT\n  hsts: false\n- host: app.flora.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:47:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: florafauna.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: flora.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flora-fauna/refs/heads/main/security/flora-fauna-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Creative AI
- Generative AI
- Infinite Canvas
- Node-Based Workflows
- Creative Workspace
- Image Generation
- Video Generation
- Text-to-Image
- Text-to-Video
- AI Agents
- Multimodal AI
- Design Tools
- Creative Professionals
- Advertising
- Film
- Fashion
- Branding
- VFX
- Photography
- Architecture
- Motion Design
- FAUNA
- MCP
- Agent Tools
- Workflow Automation
---
