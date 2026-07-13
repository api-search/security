---
api_specs:
- filename: ai21-labs-asyncapi.yml
  format: yaml
  label: AI21 Jamba Chat Completions API
  slug: chat-completions
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai21-labs/refs/heads/main/asyncapi/ai21-labs-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ai21.com
  spf: true
hosts:
- cert_expires: Sep  7 01:26:06 2026 GMT
  host: www.ai21.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 19:05:04 2026 GMT
  host: docs.ai21.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 23:32:59 2026 GMT
  host: api.ai21.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ai21 Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI21 Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AI21 Labs
provider_slug: ai21-labs
slug: ai21-labs-domain-security
source_filename: ai21-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ai21.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 01:26:06 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.ai21.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 19:05:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.ai21.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 23:32:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ai21.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ai21-labs/refs/heads/main/security/ai21-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Foundation Models
- LLM
- Jamba
- Mamba
- RAG
- Agents
- Maestro
- Inference
- Enterprise AI
- Fine-Tuning
---
