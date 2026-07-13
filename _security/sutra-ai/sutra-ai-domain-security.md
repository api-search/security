---
api_specs:
- filename: sutra-ai-openapi.yml
  format: yaml
  label: SUTRA Chat Completions (Multilingual) API
  slug: chat-completions-multilingual-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sutra-ai/refs/heads/main/openapi/sutra-ai-openapi.yml
- filename: sutra-ai-openapi.yml
  format: yaml
  label: SUTRA Reasoning API
  slug: reasoning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sutra-ai/refs/heads/main/openapi/sutra-ai-openapi.yml
- filename: sutra-ai-openapi.yml
  format: yaml
  label: SUTRA Models API
  slug: models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sutra-ai/refs/heads/main/openapi/sutra-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: two.ai
  spf: true
hosts:
- cert_expires: Sep 22 01:58:50 2026 GMT
  host: www.two.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 03:40:01 2026 GMT
  host: docs.two.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.two.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Sutra Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SUTRA (Two AI), probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SUTRA (Two AI)
provider_slug: sutra-ai
slug: sutra-ai-domain-security
source_filename: sutra-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.two.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 01:58:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.two.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 03:40:01 2026 GMT\n  hsts: false\n- host: api.two.ai\n  https: false\ndomains:\n- domain: two.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sutra-ai/refs/heads/main/security/sutra-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Multilingual
- Inference
- Reasoning
---
