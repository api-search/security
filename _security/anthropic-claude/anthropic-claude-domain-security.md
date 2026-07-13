---
api_specs:
- filename: anthropic-claude-openapi.yml
  format: yaml
  label: Anthropic Claude Messages API
  slug: messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic-claude/refs/heads/main/openapi/anthropic-claude-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: anthropic.com
  spf: true
hosts:
- cert_expires: Oct  6 15:03:46 2026 GMT
  host: www.anthropic.com
  hsts: true
  hsts_max_age: 3600
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
name: Anthropic Claude Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anthropic Claude, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Anthropic Claude
provider_slug: anthropic-claude
slug: anthropic-claude-domain-security
source_filename: anthropic-claude-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anthropic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 15:03:46 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\n- host: docs.anthropic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 19:48:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.anthropic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 18:45:51 2026 GMT\n  hsts: null\ndomains:\n- domain: anthropic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anthropic-claude/refs/heads/main/security/anthropic-claude-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Large Language Models
- LLM
- Generative AI
- Chat
- Agents
- Claude
---
