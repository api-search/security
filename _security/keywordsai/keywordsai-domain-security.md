---
api_specs:
- filename: keywordsai-openapi.yml
  format: yaml
  label: Keywords AI LLM Proxy (Chat Completions)
  slug: llm-proxy-chat-completions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-openapi.yml
- filename: keywordsai-openapi.yml
  format: yaml
  label: Keywords AI Logging API
  slug: logging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-openapi.yml
- filename: keywordsai-openapi.yml
  format: yaml
  label: Keywords AI Prompts API
  slug: prompts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-openapi.yml
- filename: keywordsai-openapi.yml
  format: yaml
  label: Keywords AI Threads API
  slug: threads
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-openapi.yml
- filename: keywordsai-openapi.yml
  format: yaml
  label: Keywords AI Evaluations API
  slug: evaluations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-openapi.yml
- filename: keywordsai-openapi.yml
  format: yaml
  label: Keywords AI Traces API
  slug: traces
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: keywordsai.co
  spf: true
hosts:
- cert_expires: Sep 23 13:52:48 2026 GMT
  host: www.keywordsai.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 17:10:50 2026 GMT
  host: docs.keywordsai.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: api.keywordsai.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keywordsai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keywords AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Keywords AI
provider_slug: keywordsai
slug: keywordsai-domain-security
source_filename: keywordsai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.keywordsai.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 13:52:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.keywordsai.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 17:10:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.keywordsai.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: keywordsai.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/security/keywordsai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Observability
- Gateway
- Monitoring
---
