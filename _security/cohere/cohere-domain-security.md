---
api_specs:
- filename: cohere-chat-api-openapi.yml
  format: yaml
  label: Cohere Chat API
  slug: chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/openapi/cohere-chat-api-openapi.yml
- filename: cohere-embed-api-openapi.yml
  format: yaml
  label: Cohere Embed API
  slug: embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/openapi/cohere-embed-api-openapi.yml
- filename: cohere-rerank-api-openapi.yml
  format: yaml
  label: Cohere Rerank API
  slug: rerank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/openapi/cohere-rerank-api-openapi.yml
- filename: cohere-classify-api-openapi.yml
  format: yaml
  label: Cohere Classify API
  slug: classify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/openapi/cohere-classify-api-openapi.yml
- filename: cohere-embed-jobs-api-openapi.yml
  format: yaml
  label: Cohere Embed Jobs API
  slug: embed-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/openapi/cohere-embed-jobs-api-openapi.yml
- filename: cohere-datasets-api-openapi.yml
  format: yaml
  label: Cohere Datasets API
  slug: datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/openapi/cohere-datasets-api-openapi.yml
- filename: cohere-models-api-openapi.yml
  format: yaml
  label: Cohere Models API
  slug: models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/openapi/cohere-models-api-openapi.yml
- filename: cohere-tokenize-api-openapi.yml
  format: yaml
  label: Cohere Tokenize API
  slug: tokenize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/openapi/cohere-tokenize-api-openapi.yml
- filename: cohere-detokenize-api-openapi.yml
  format: yaml
  label: Cohere Detokenize API
  slug: detokenize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/openapi/cohere-detokenize-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cohere.com
  spf: true
hosts:
- cert_expires: Sep 26 05:19:39 2026 GMT
  host: docs.cohere.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 12:46:59 2026 GMT
  host: api.cohere.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cohere Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for cohere, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: cohere
provider_slug: cohere
slug: cohere-domain-security
source_filename: cohere-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.cohere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 05:19:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cohere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 12:46:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cohere.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cohere/refs/heads/main/security/cohere-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
