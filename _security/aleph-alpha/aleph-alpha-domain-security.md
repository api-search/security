---
api_specs:
- filename: aleph-alpha-pharia-inference-openapi.json
  format: json
  label: PhariaInference API
  slug: pharia-inference
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha/refs/heads/main/openapi/aleph-alpha-pharia-inference-openapi.json
- filename: aleph-alpha-pharia-data-openapi.json
  format: json
  label: PhariaData API
  slug: pharia-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha/refs/heads/main/openapi/aleph-alpha-pharia-data-openapi.json
- filename: aleph-alpha-pharia-search-openapi.json
  format: json
  label: PhariaSearch / Document Index API
  slug: pharia-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha/refs/heads/main/openapi/aleph-alpha-pharia-search-openapi.json
- filename: aleph-alpha-pharia-studio-openapi.json
  format: json
  label: PhariaStudio API
  slug: pharia-studio
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha/refs/heads/main/openapi/aleph-alpha-pharia-studio-openapi.json
- filename: aleph-alpha-pharia-os-openapi.json
  format: json
  label: PhariaOS Manager API
  slug: pharia-os
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha/refs/heads/main/openapi/aleph-alpha-pharia-os-openapi.json
- filename: aleph-alpha-responses-openapi.json
  format: json
  label: Responses API (Stateful Responses)
  slug: responses
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha/refs/heads/main/openapi/aleph-alpha-responses-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aleph-alpha.com
  spf: true
hosts:
- cert_expires: Sep  2 04:14:01 2026 GMT
  host: aleph-alpha.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 06:16:25 2026 GMT
  host: docs.aleph-alpha.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 16:28:07 2026 GMT
  host: api.aleph-alpha.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aleph Alpha Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aleph Alpha, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aleph Alpha
provider_slug: aleph-alpha
slug: aleph-alpha-domain-security
source_filename: aleph-alpha-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aleph-alpha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 04:14:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.aleph-alpha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 06:16:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.aleph-alpha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 16:28:07 2026 GMT\n  hsts: null\ndomains:\n- domain: aleph-alpha.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aleph-alpha/refs/heads/main/security/aleph-alpha-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Large Language Models
- Generative AI
- Sovereign AI
- Inference
- Embeddings
- Semantic Search
- Vector Search
- Agents
- Model Context Protocol
- Germany
- Enterprise Software
- Government
---
