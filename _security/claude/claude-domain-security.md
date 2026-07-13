---
api_specs:
- filename: claude-messages-api.yml
  format: yaml
  label: Claude Messages API
  slug: claude-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/openapi/claude-messages-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: anthropic.com
  spf: true
hosts:
- cert_expires: Sep  5 05:27:10 2026 GMT
  host: console.anthropic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 19:48:08 2026 GMT
  host: docs.anthropic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 18:45:51 2026 GMT
  host: api.anthropic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Claude Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Claude, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Claude
provider_slug: claude
slug: claude-domain-security
source_filename: claude-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: console.anthropic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 05:27:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.anthropic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 19:48:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.anthropic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 18:45:51 2026 GMT\n  hsts: null\ndomains:\n- domain: anthropic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/security/claude-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
---
