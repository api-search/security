---
api_specs:
- filename: freeplay-agents-api-openapi.yml
  format: yaml
  label: Freeplay Agents API
  slug: freeplay-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-agents-api-openapi.yml
- filename: freeplay-prompt-templates-api-openapi.yml
  format: yaml
  label: Freeplay Prompt Templates API
  slug: freeplay-prompt-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-prompt-templates-api-openapi.yml
- filename: freeplay-test-runs-api-openapi.yml
  format: yaml
  label: Freeplay Test Runs API
  slug: freeplay-test-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-test-runs-api-openapi.yml
- filename: freeplay-agent-datasets-api-openapi.yml
  format: yaml
  label: Freeplay Agent Datasets API
  slug: freeplay-agent-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-agent-datasets-api-openapi.yml
- filename: freeplay-configuration-api-openapi.yml
  format: yaml
  label: Freeplay Configuration API
  slug: freeplay-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-configuration-api-openapi.yml
- filename: freeplay-evaluation-criteria-api-openapi.yml
  format: yaml
  label: Freeplay Evaluation Criteria API
  slug: freeplay-evaluation-criteria-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-evaluation-criteria-api-openapi.yml
- filename: freeplay-insights-api-openapi.yml
  format: yaml
  label: Freeplay Insights API
  slug: freeplay-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-insights-api-openapi.yml
- filename: freeplay-models-api-openapi.yml
  format: yaml
  label: Freeplay Models API
  slug: freeplay-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-models-api-openapi.yml
- filename: freeplay-observability-api-openapi.yml
  format: yaml
  label: Freeplay Observability API
  slug: freeplay-observability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-observability-api-openapi.yml
- filename: freeplay-prompt-datasets-api-openapi.yml
  format: yaml
  label: Freeplay Prompt Datasets API
  slug: freeplay-prompt-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-prompt-datasets-api-openapi.yml
- filename: freeplay-prompt-optimization-api-openapi.yml
  format: yaml
  label: Freeplay Prompt Optimization API
  slug: freeplay-prompt-optimization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-prompt-optimization-api-openapi.yml
- filename: freeplay-review-queues-api-openapi.yml
  format: yaml
  label: Freeplay Review Queues API
  slug: freeplay-review-queues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-review-queues-api-openapi.yml
- filename: freeplay-saved-searches-api-openapi.yml
  format: yaml
  label: Freeplay Saved Searches API
  slug: freeplay-saved-searches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-saved-searches-api-openapi.yml
- filename: freeplay-search-analytics-api-openapi.yml
  format: yaml
  label: Freeplay Search & Analytics API
  slug: freeplay-search-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-search-analytics-api-openapi.yml
- filename: freeplay-tags-api-openapi.yml
  format: yaml
  label: Freeplay Tags API
  slug: freeplay-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeplay/openapi/freeplay-tags-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: freeplay.ai
  spf: true
hosts:
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: freeplay.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 09:36:02 2026 GMT
  host: docs.freeplay.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 10:56:52 2026 GMT
  host: app.freeplay.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Freeplay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freeplay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Freeplay
provider_slug: freeplay
slug: freeplay-domain-security
source_filename: freeplay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freeplay.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: null\n- host: docs.freeplay.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 09:36:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.freeplay.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 10:56:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: freeplay.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/freeplay/security/freeplay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- LLM
- Evaluation
- Observability
- Prompt Management
- Experimentation
---
