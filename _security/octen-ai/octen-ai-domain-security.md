---
api_specs:
- filename: octen-ai-answer-api-openapi.yml
  format: yaml
  label: Octen Answer API
  slug: octen-ai-answer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-answer-api-openapi.yml
- filename: octen-ai-broad-search-api-openapi.yml
  format: yaml
  label: Octen Broad Search API
  slug: octen-ai-broad-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-broad-search-api-openapi.yml
- filename: octen-ai-business-search-api-openapi.yml
  format: yaml
  label: Octen Business Search API
  slug: octen-ai-business-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-business-search-api-openapi.yml
- filename: octen-ai-embedding-api-openapi.yml
  format: yaml
  label: Octen Embedding API
  slug: octen-ai-embedding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-embedding-api-openapi.yml
- filename: octen-ai-extract-api-openapi.yml
  format: yaml
  label: Octen Extract API
  slug: octen-ai-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-extract-api-openapi.yml
- filename: octen-ai-grounded-generation-api-openapi.yml
  format: yaml
  label: Octen Grounded Generation API
  slug: octen-ai-grounded-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-grounded-generation-api-openapi.yml
- filename: octen-ai-image-search-api-openapi.yml
  format: yaml
  label: Octen Image Search API
  slug: octen-ai-image-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-image-search-api-openapi.yml
- filename: octen-ai-images-api-openapi.yml
  format: yaml
  label: Octen Images API
  slug: octen-ai-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-images-api-openapi.yml
- filename: octen-ai-messages-api-openapi.yml
  format: yaml
  label: Octen Messages API
  slug: octen-ai-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-messages-api-openapi.yml
- filename: octen-ai-news-search-api-openapi.yml
  format: yaml
  label: Octen News Search API
  slug: octen-ai-news-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-news-search-api-openapi.yml
- filename: octen-ai-research-api-openapi.yml
  format: yaml
  label: Octen Research API
  slug: octen-ai-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-research-api-openapi.yml
- filename: octen-ai-search-api-openapi.yml
  format: yaml
  label: Octen Search API
  slug: octen-ai-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-search-api-openapi.yml
- filename: octen-ai-video-search-api-openapi.yml
  format: yaml
  label: Octen Video Search API
  slug: octen-ai-video-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-video-search-api-openapi.yml
- filename: octen-ai-videos-api-openapi.yml
  format: yaml
  label: Octen Videos API
  slug: octen-ai-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-videos-api-openapi.yml
- filename: octen-ai-vl-embedding-api-openapi.yml
  format: yaml
  label: Octen Vl Embedding API
  slug: octen-ai-vl-embedding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-vl-embedding-api-openapi.yml
- filename: octen-ai-chat-completions-api-openapi.yml
  format: yaml
  label: Octen Chat Completions API
  slug: octen-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-chat-completions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 iodef "mailto:security@octen.ai"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "godaddy.com"
  - 0 issue "starfieldtech.com"
  dmarc: true
  dnssec: false
  domain: octen.ai
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: octen.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Octen Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Octen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: Octen
provider_slug: octen-ai
slug: octen-ai-domain-security
source_filename: octen-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: octen.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: octen.ai\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 iodef \"mailto:security@octen.ai\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"starfieldtech.com\"\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/security/octen-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Search
- Web Search
- AI
- LLM
- Embeddings
- Content Extraction
- Model Gateway
- MCP
- Agents
- Deep Research
- Company
---
