---
api_specs:
- filename: vectara-openapi.yml
  format: yaml
  label: Vectara REST API
  slug: vectara-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/openapi/vectara-openapi.yml
- filename: vectara-openapi.yml
  format: yaml
  label: Vectara Corpora API
  slug: vectara-corpora-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/openapi/vectara-openapi.yml
- filename: vectara-openapi.yml
  format: yaml
  label: Vectara Indexing API
  slug: vectara-indexing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/openapi/vectara-openapi.yml
- filename: vectara-openapi.yml
  format: yaml
  label: Vectara Query API
  slug: vectara-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/openapi/vectara-openapi.yml
- filename: vectara-openapi.yml
  format: yaml
  label: Vectara Agents API
  slug: vectara-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/openapi/vectara-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: vectara.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: vectara.io
  spf: false
hosts:
- cert_expires: Oct  4 20:52:20 2026 GMT
  host: www.vectara.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 17:15:19 2026 GMT
  host: docs.vectara.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 09:03:05 2026 GMT
  host: api.vectara.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vectara Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vectara, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Vectara
provider_slug: vectara
slug: vectara-domain-security
source_filename: vectara-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vectara.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 20:52:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.vectara.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 17:15:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.vectara.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 09:03:05 2026 GMT\n  hsts: null\ndomains:\n- domain: vectara.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: vectara.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vectara/refs/heads/main/security/vectara-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Agents
- Corpora
- Embeddings
- Enterprise Search
- Generative AI
- Grounded Generation
- Hallucination Detection
- LLM
- MCP
- RAG
- Retrieval
- Search
- Semantic Search
- Vector Search
---
