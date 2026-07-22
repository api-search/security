---
api_specs:
- filename: napkinai-openapi.yml
  format: yaml
  label: Napkin AI API
  slug: napkin-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/napkinai/refs/heads/main/openapi/napkinai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: napkin.ai
  spf: true
hosts:
- cert_expires: Sep 20 20:47:14 2026 GMT
  host: www.napkin.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 03:14:28 2026 GMT
  host: api.napkin.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Napkinai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Napkin.AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Napkin.AI
provider_slug: napkinai
slug: napkinai-domain-security
source_filename: napkinai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.napkin.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 20:47:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.napkin.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 03:14:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: napkin.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/napkinai/refs/heads/main/security/napkinai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Visualization
- Diagrams
- Charts
- Infographics
- Presentations
- Content Generation
- Design
- Developer API
---
