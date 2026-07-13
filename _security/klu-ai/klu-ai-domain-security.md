---
api_specs:
- filename: klu-ai-openapi.yml
  format: yaml
  label: Klu Actions / Prompt API
  slug: klu-actions-prompt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klu-ai/refs/heads/main/openapi/klu-ai-openapi.yml
- filename: klu-ai-openapi.yml
  format: yaml
  label: Klu Data / Feedback API
  slug: klu-data-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klu-ai/refs/heads/main/openapi/klu-ai-openapi.yml
- filename: klu-ai-openapi.yml
  format: yaml
  label: Klu Models API
  slug: klu-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klu-ai/refs/heads/main/openapi/klu-ai-openapi.yml
- filename: klu-ai-openapi.yml
  format: yaml
  label: Klu Sessions API
  slug: klu-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klu-ai/refs/heads/main/openapi/klu-ai-openapi.yml
- filename: klu-ai-openapi.yml
  format: yaml
  label: Klu Apps / Workspaces API
  slug: klu-apps-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klu-ai/refs/heads/main/openapi/klu-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: true
  domain: klu.ai
  spf: true
hosts:
- cert_expires: Oct  4 01:25:26 2026 GMT
  host: klu.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 01:25:26 2026 GMT
  host: docs.klu.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 01:25:26 2026 GMT
  host: api.klu.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Klu Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Klu, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present.'
provider_name: Klu
provider_slug: klu-ai
slug: klu-ai-domain-security
source_filename: klu-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: klu.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 01:25:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.klu.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 01:25:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.klu.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 01:25:26 2026 GMT\n  hsts: null\ndomains:\n- domain: klu.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klu-ai/refs/heads/main/security/klu-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- LLM
- LLM App Platform
- Prompt Engineering
- Evaluation
- Observability
---
