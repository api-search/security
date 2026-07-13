---
api_specs:
- filename: jina-ai-embeddings-openapi.yml
  format: yaml
  label: Jina AI Embeddings API
  slug: embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jina-ai/refs/heads/main/openapi/jina-ai-embeddings-openapi.yml
- filename: jina-ai-reader-openapi.yml
  format: yaml
  label: Jina AI Reader API
  slug: reader-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jina-ai/refs/heads/main/openapi/jina-ai-reader-openapi.yml
- filename: jina-ai-reranker-openapi.yml
  format: yaml
  label: Jina AI Reranker API
  slug: reranker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jina-ai/refs/heads/main/openapi/jina-ai-reranker-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jina.ai
  spf: true
hosts:
- cert_expires: Oct  1 12:12:38 2026 GMT
  host: jina.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 07:03:02 2026 GMT
  host: api.jina.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 07:03:02 2026 GMT
  host: r.jina.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jina Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jina AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jina AI
provider_slug: jina-ai
slug: jina-ai-domain-security
source_filename: jina-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jina.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 12:12:38 2026 GMT\n  hsts: false\n- host: api.jina.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 07:03:02 2026 GMT\n  hsts: null\n- host: r.jina.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 07:03:02 2026 GMT\n  hsts: null\ndomains:\n- domain: jina.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jina-ai/refs/heads/main/security/jina-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Embeddings
- Machine Learning
- Reranking
- Search
---
