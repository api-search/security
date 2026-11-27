---
api_specs:
- filename: clipspeed-ai-openapi-generated.yml
  format: yaml
  label: ClipSpeed API
  slug: clipspeed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipspeed-ai/openapi/_ae-authored/clipspeed-ai-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clipspeed.ai
  spf: true
hosts:
- cert_expires: Jan 26 18:00:30 2027 GMT
  host: clipspeed.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ClipSpeedAI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClipSpeedAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ClipSpeedAI
provider_slug: clipspeed-ai
slug: clipspeed-ai-domain-security
source_filename: clipspeed-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clipspeed.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 18:00:30 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: clipspeed.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/clipspeed-ai/security/clipspeed-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Video
- Video Clipping
- Image Generation
- Generative AI
- Live Streaming
- Social Media
- MCP
---
