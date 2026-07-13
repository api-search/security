---
api_specs:
- filename: promptlayer-openapi.yml
  format: yaml
  label: PromptLayer Request Logging & Tracking API
  slug: request-logging-tracking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/promptlayer/refs/heads/main/openapi/promptlayer-openapi.yml
- filename: promptlayer-openapi.yml
  format: yaml
  label: PromptLayer Prompt Registry & Templates API
  slug: prompt-registry-templates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/promptlayer/refs/heads/main/openapi/promptlayer-openapi.yml
- filename: promptlayer-openapi.yml
  format: yaml
  label: PromptLayer Evaluations & Datasets API
  slug: evaluations-datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/promptlayer/refs/heads/main/openapi/promptlayer-openapi.yml
- filename: promptlayer-openapi.yml
  format: yaml
  label: PromptLayer Spans & Traces API
  slug: spans-traces
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/promptlayer/refs/heads/main/openapi/promptlayer-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: promptlayer.com
  spf: true
hosts:
- cert_expires: Aug 15 09:21:27 2026 GMT
  host: www.promptlayer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 00:55:57 2026 GMT
  host: docs.promptlayer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 18:10:04 2026 GMT
  host: api.promptlayer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Promptlayer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PromptLayer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: PromptLayer
provider_slug: promptlayer
slug: promptlayer-domain-security
source_filename: promptlayer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.promptlayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 09:21:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.promptlayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 00:55:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.promptlayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 18:10:04 2026 GMT\n  hsts: null\ndomains:\n- domain: promptlayer.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/promptlayer/refs/heads/main/security/promptlayer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- LLM
- Prompt Engineering
- Prompt Management
- Observability
- Evaluation
---
