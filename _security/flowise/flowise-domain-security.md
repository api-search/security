---
api_specs:
- filename: flowise-openapi.yml
  format: yaml
  label: Flowise API
  slug: flowise
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flowiseai.com
  spf: true
hosts:
- cert_expires: Aug 21 09:49:24 2026 GMT
  host: flowiseai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 03:02:32 2026 GMT
  host: docs.flowiseai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flowise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flowise, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flowise
provider_slug: flowise
slug: flowise-domain-security
source_filename: flowise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flowiseai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 09:49:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.flowiseai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 03:02:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flowiseai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/security/flowise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- Agent Workflows
- Artificial Intelligence
- Large Language Models
- Low Code
- Visual Builder
- LangChain
- RAG
- Retrieval Augmented Generation
- Chatbots
- Open Source
- Node.js
- TypeScript
---
