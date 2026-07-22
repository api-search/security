---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: florafauna.ai
  spf: true
hosts:
- cert_expires: Oct  4 23:54:55 2026 GMT
  host: www.florafauna.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flora Fauna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FLORA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FLORA
provider_slug: flora-fauna
slug: flora-fauna-domain-security
source_filename: flora-fauna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.florafauna.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:54:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: florafauna.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
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
---
