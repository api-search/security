---
api_specs:
- filename: perplexity-asyncapi.yml
  format: yaml
  label: Perplexity Async Chat Completions API
  slug: async-chat-completions-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/asyncapi/perplexity-asyncapi.yml
- filename: perplexity-asyncapi.yml
  format: yaml
  label: Perplexity Responses API
  slug: responses-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/asyncapi/perplexity-asyncapi.yml
- filename: perplexity-agent-api-openapi.yml
  format: yaml
  label: Perplexity Agent API
  slug: perplexity-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/openapi/perplexity-agent-api-openapi.yml
- filename: perplexity-async-api-openapi.yml
  format: yaml
  label: Perplexity Async API
  slug: perplexity-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/openapi/perplexity-async-api-openapi.yml
- filename: perplexity-contextualizedembeddings-api-openapi.yml
  format: yaml
  label: Perplexity Contextualizedembeddings API
  slug: perplexity-contextualizedembeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/openapi/perplexity-contextualizedembeddings-api-openapi.yml
- filename: perplexity-embeddings-api-openapi.yml
  format: yaml
  label: Perplexity Embeddings API
  slug: perplexity-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/openapi/perplexity-embeddings-api-openapi.yml
- filename: perplexity-models-api-openapi.yml
  format: yaml
  label: Perplexity Models API
  slug: perplexity-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/openapi/perplexity-models-api-openapi.yml
- filename: perplexity-search-api-openapi.yml
  format: yaml
  label: Perplexity Search API
  slug: perplexity-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/openapi/perplexity-search-api-openapi.yml
- filename: perplexity-sonar-api-openapi.yml
  format: yaml
  label: Perplexity Sonar API
  slug: perplexity-sonar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/openapi/perplexity-sonar-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: perplexity.ai
  spf: true
hosts:
- cert_expires: Sep 15 15:11:24 2026 GMT
  host: www.perplexity.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 17:06:38 2026 GMT
  host: docs.perplexity.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 15:11:24 2026 GMT
  host: api.perplexity.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Perplexity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perplexity, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Perplexity
provider_slug: perplexity
slug: perplexity-domain-security
source_filename: perplexity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.perplexity.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 15:11:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.perplexity.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 17:06:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.perplexity.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 15:11:24 2026 GMT\n  hsts: null\ndomains:\n- domain: perplexity.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/security/perplexity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
