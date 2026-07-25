---
api_specs:
- filename: openpipe-chat-api-openapi.yml
  format: yaml
  label: OpenPipe Chat API
  slug: openpipe-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/openapi/openpipe-chat-api-openapi.yml
- filename: openpipe-check-cache-api-openapi.yml
  format: yaml
  label: OpenPipe Check Cache API
  slug: openpipe-check-cache-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/openapi/openpipe-check-cache-api-openapi.yml
- filename: openpipe-criteria-api-openapi.yml
  format: yaml
  label: OpenPipe Criteria API
  slug: openpipe-criteria-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/openapi/openpipe-criteria-api-openapi.yml
- filename: openpipe-datasets-api-openapi.yml
  format: yaml
  label: OpenPipe Datasets API
  slug: openpipe-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/openapi/openpipe-datasets-api-openapi.yml
- filename: openpipe-local-testing-only-get-latest-logged-call-api-openapi.yml
  format: yaml
  label: OpenPipe Local Testing Only Get Latest Logged Call API
  slug: openpipe-local-testing-only-get-latest-logged-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/openapi/openpipe-local-testing-only-get-latest-logged-call-api-openapi.yml
- filename: openpipe-logs-api-openapi.yml
  format: yaml
  label: OpenPipe Logs API
  slug: openpipe-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/openapi/openpipe-logs-api-openapi.yml
- filename: openpipe-models-api-openapi.yml
  format: yaml
  label: OpenPipe Models API
  slug: openpipe-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/openapi/openpipe-models-api-openapi.yml
- filename: openpipe-report-anthropic-api-openapi.yml
  format: yaml
  label: OpenPipe Report Anthropic API
  slug: openpipe-report-anthropic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/openapi/openpipe-report-anthropic-api-openapi.yml
- filename: openpipe-report-api-openapi.yml
  format: yaml
  label: OpenPipe Report API
  slug: openpipe-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/openapi/openpipe-report-api-openapi.yml
- filename: openpipe-unstable-api-openapi.yml
  format: yaml
  label: OpenPipe Unstable API
  slug: openpipe-unstable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/openapi/openpipe-unstable-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: openpipe.ai
  spf: true
hosts:
- cert_expires: Sep 21 20:13:51 2026 GMT
  host: openpipe.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 15:51:18 2026 GMT
  host: docs.openpipe.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: api.openpipe.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openpipe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenPipe, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OpenPipe
provider_slug: openpipe
slug: openpipe-domain-security
source_filename: openpipe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openpipe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 20:13:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.openpipe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 15:51:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.openpipe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openpipe.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openpipe/refs/heads/main/security/openpipe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Fine-Tuning
- Distillation
- Inference
- OpenAI Compatible
- Anthropic Compatible
- Caching
---
