---
api_specs:
- filename: compoid-com-completions-api-openapi.yml
  format: yaml
  label: Compoid Completions API
  slug: compoid-com-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-completions-api-openapi.yml
- filename: compoid-com-detokenize-api-openapi.yml
  format: yaml
  label: Compoid Detokenize API
  slug: compoid-com-detokenize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-detokenize-api-openapi.yml
- filename: compoid-com-generative-scoring-api-openapi.yml
  format: yaml
  label: Compoid Generative Scoring API
  slug: compoid-com-generative-scoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-generative-scoring-api-openapi.yml
- filename: compoid-com-health-api-openapi.yml
  format: yaml
  label: Compoid Health API
  slug: compoid-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-health-api-openapi.yml
- filename: compoid-com-invocations-api-openapi.yml
  format: yaml
  label: Compoid Invocations API
  slug: compoid-com-invocations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-invocations-api-openapi.yml
- filename: compoid-com-is-scaling-elastic-ep-api-openapi.yml
  format: yaml
  label: Compoid Is Scaling Elastic Ep API
  slug: compoid-com-is-scaling-elastic-ep-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-is-scaling-elastic-ep-api-openapi.yml
- filename: compoid-com-kv-event-sources-api-openapi.yml
  format: yaml
  label: Compoid Kv Event Sources API
  slug: compoid-com-kv-event-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-kv-event-sources-api-openapi.yml
- filename: compoid-com-load-api-openapi.yml
  format: yaml
  label: Compoid Load API
  slug: compoid-com-load-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-load-api-openapi.yml
- filename: compoid-com-messages-api-openapi.yml
  format: yaml
  label: Compoid Messages API
  slug: compoid-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-messages-api-openapi.yml
- filename: compoid-com-metrics-api-openapi.yml
  format: yaml
  label: Compoid Metrics API
  slug: compoid-com-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-metrics-api-openapi.yml
- filename: compoid-com-models-api-openapi.yml
  format: yaml
  label: Compoid Models API
  slug: compoid-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-models-api-openapi.yml
- filename: compoid-com-ping-api-openapi.yml
  format: yaml
  label: Compoid Ping API
  slug: compoid-com-ping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-ping-api-openapi.yml
- filename: compoid-com-responses-api-openapi.yml
  format: yaml
  label: Compoid Responses API
  slug: compoid-com-responses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-responses-api-openapi.yml
- filename: compoid-com-scale-elastic-ep-api-openapi.yml
  format: yaml
  label: Compoid Scale Elastic Ep API
  slug: compoid-com-scale-elastic-ep-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-scale-elastic-ep-api-openapi.yml
- filename: compoid-com-systemone-api-openapi.yml
  format: yaml
  label: Compoid Systemone API
  slug: compoid-com-systemone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-systemone-api-openapi.yml
- filename: compoid-com-tokenize-api-openapi.yml
  format: yaml
  label: Compoid Tokenize API
  slug: compoid-com-tokenize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-tokenize-api-openapi.yml
- filename: compoid-com-version-api-openapi.yml
  format: yaml
  label: Compoid Version API
  slug: compoid-com-version-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-version-api-openapi.yml
- filename: compoid-com-chat-completions-api-openapi.yml
  format: yaml
  label: Compoid Chat Completions API
  slug: compoid-com-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compoid-com/openapi/compoid-com-chat-completions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: compoid.com
  spf: true
hosts:
- cert_expires: Jan  2 11:13:08 2027 GMT
  host: compoid.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Compoid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Compoid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Compoid
provider_slug: compoid-com
slug: compoid-com-domain-security
source_filename: compoid-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: compoid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 11:13:08 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: compoid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/compoid-com/security/compoid-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- MCP
- Digital Repository
- Research Data
- Datasets
- Knowledge Management
- Agent Memory
---
