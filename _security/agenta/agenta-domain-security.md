---
api_specs:
- filename: agenta-openapi.yml
  format: yaml
  label: Agenta Apps and Variants API
  slug: agenta-apps-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agenta/refs/heads/main/openapi/agenta-openapi.yml
- filename: agenta-openapi.yml
  format: yaml
  label: Agenta Configs and Prompts API
  slug: agenta-configs-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agenta/refs/heads/main/openapi/agenta-openapi.yml
- filename: agenta-openapi.yml
  format: yaml
  label: Agenta Evaluations and Evaluators API
  slug: agenta-evaluations-evaluators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agenta/refs/heads/main/openapi/agenta-openapi.yml
- filename: agenta-openapi.yml
  format: yaml
  label: Agenta Testsets API
  slug: agenta-testsets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agenta/refs/heads/main/openapi/agenta-openapi.yml
- filename: agenta-openapi.yml
  format: yaml
  label: Agenta Observability and Traces API
  slug: agenta-observability-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agenta/refs/heads/main/openapi/agenta-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agenta.ai
  spf: true
hosts:
- cert_expires: Oct  6 11:58:16 2026 GMT
  host: agenta.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 19:04:36 2026 GMT
  host: docs.agenta.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: cloud.agenta.ai
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Agenta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agenta, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agenta
provider_slug: agenta
slug: agenta-domain-security
source_filename: agenta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agenta.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 11:58:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.agenta.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 19:04:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cloud.agenta.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: agenta.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agenta/refs/heads/main/security/agenta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLMOps
- Prompt Management
- LLM Evaluation
- Observability
---
