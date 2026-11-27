---
api_specs:
- filename: perplexity-asyncapi.yml
  format: yaml
  label: Perplexity Async Chat Completions API
  slug: async-chat-completions-api
  spec_type: AsyncAPI
  url: https://artifacts.apis.io/perplexity/asyncapi/perplexity-asyncapi.yml
- filename: perplexity-asyncapi.yml
  format: yaml
  label: Perplexity Responses API
  slug: responses-api
  spec_type: AsyncAPI
  url: https://artifacts.apis.io/perplexity/asyncapi/perplexity-asyncapi.yml
- filename: perplexity-agent-api-openapi.yml
  format: yaml
  label: Perplexity Agent API
  slug: perplexity-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/perplexity/openapi/perplexity-agent-api-openapi.yml
- filename: perplexity-async-api-openapi.yml
  format: yaml
  label: Perplexity Async API
  slug: perplexity-async-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/perplexity/openapi/perplexity-async-api-openapi.yml
- filename: perplexity-contextualizedembeddings-api-openapi.yml
  format: yaml
  label: Perplexity Contextualizedembeddings API
  slug: perplexity-contextualizedembeddings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/perplexity/openapi/perplexity-contextualizedembeddings-api-openapi.yml
- filename: perplexity-embeddings-api-openapi.yml
  format: yaml
  label: Perplexity Embeddings API
  slug: perplexity-embeddings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/perplexity/openapi/perplexity-embeddings-api-openapi.yml
- filename: perplexity-models-api-openapi.yml
  format: yaml
  label: Perplexity Models API
  slug: perplexity-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/perplexity/openapi/perplexity-models-api-openapi.yml
- filename: perplexity-search-api-openapi.yml
  format: yaml
  label: Perplexity Search API
  slug: perplexity-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/perplexity/openapi/perplexity-search-api-openapi.yml
- filename: perplexity-decisions-api-openapi.yml
  format: yaml
  label: Perplexity Decisions API
  slug: perplexity-decisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/perplexity/openapi/perplexity-decisions-api-openapi.yml
- filename: perplexity-sonar-api-openapi.yml
  format: yaml
  label: Perplexity Sonar API
  slug: perplexity-sonar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/perplexity/openapi/perplexity-sonar-api-openapi.yml
- filename: perplexity-admin-api-openapi.yml
  format: yaml
  label: Perplexity Admin API
  slug: perplexity-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/perplexity/openapi/perplexity-admin-api-openapi.yml
- filename: perplexity-analytics-api-openapi.yml
  format: yaml
  label: Perplexity Analytics API
  slug: perplexity-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/perplexity/openapi/perplexity-analytics-api-openapi.yml
- filename: perplexity-batches-api-openapi.yml
  format: yaml
  label: Perplexity Batches API
  slug: perplexity-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/perplexity/openapi/perplexity-batches-api-openapi.yml
- filename: perplexity-skills-api-openapi.yml
  format: yaml
  label: Perplexity Skills API
  slug: perplexity-skills-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/perplexity/openapi/perplexity-skills-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: perplexity.ai
  spf: true
hosts:
- cert_expires: Jan 11 14:20:34 2027 GMT
  host: www.perplexity.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 20:16:52 2026 GMT
  host: docs.perplexity.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 11 14:20:34 2027 GMT
  host: api.perplexity.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Perplexity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perplexity, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Perplexity
provider_slug: perplexity
slug: perplexity-domain-security
source_filename: perplexity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.perplexity.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 14:20:34 2027 GMT\n  hsts: null\n- host: docs.perplexity.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 20:16:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.perplexity.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 14:20:34 2027 GMT\n  hsts: null\ndomains:\n- domain: perplexity.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/perplexity/security/perplexity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- LLM
- Search
- Agents
- Embeddings
- Research
- Agentic Commerce
- Foundation Models
---
