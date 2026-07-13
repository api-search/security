---
api_specs:
- filename: glhf-chat-openapi.yml
  format: yaml
  label: glhf Chat Completions API
  slug: glhf-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glhf-chat/refs/heads/main/openapi/glhf-chat-openapi.yml
- filename: glhf-chat-openapi.yml
  format: yaml
  label: glhf Models API
  slug: glhf-chat-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glhf-chat/refs/heads/main/openapi/glhf-chat-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: glhf.chat
  spf: true
hosts:
- cert_expires: Aug 26 18:42:33 2026 GMT
  host: glhf.chat
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glhf Chat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for glhf, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: glhf
provider_slug: glhf-chat
slug: glhf-chat-domain-security
source_filename: glhf-chat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: glhf.chat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 18:42:33 2026 GMT\n  hsts: null\ndomains:\n- domain: glhf.chat\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glhf-chat/refs/heads/main/security/glhf-chat-domain-security.yml
summary_line: TLSv1.3
tags:
- AI
- LLM
- Inference
- Open Source Models
- Hugging Face
---
