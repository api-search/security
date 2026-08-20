---
api_specs:
- filename: lightly-ai-datasets-api-openapi.yml
  format: yaml
  label: Lightly Datasets API
  slug: lightly-ai-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightly-ai/refs/heads/main/openapi/lightly-ai-datasets-api-openapi.yml
- filename: lightly-ai-datasources-api-openapi.yml
  format: yaml
  label: Lightly Datasources API
  slug: lightly-ai-datasources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightly-ai/refs/heads/main/openapi/lightly-ai-datasources-api-openapi.yml
- filename: lightly-ai-embeddings-api-openapi.yml
  format: yaml
  label: Lightly Embeddings API
  slug: lightly-ai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightly-ai/refs/heads/main/openapi/lightly-ai-embeddings-api-openapi.yml
- filename: lightly-ai-jobs-api-openapi.yml
  format: yaml
  label: Lightly Jobs API
  slug: lightly-ai-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightly-ai/refs/heads/main/openapi/lightly-ai-jobs-api-openapi.yml
- filename: lightly-ai-samples-api-openapi.yml
  format: yaml
  label: Lightly Samples API
  slug: lightly-ai-samples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightly-ai/refs/heads/main/openapi/lightly-ai-samples-api-openapi.yml
- filename: lightly-ai-selection-api-openapi.yml
  format: yaml
  label: Lightly Selection API
  slug: lightly-ai-selection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightly-ai/refs/heads/main/openapi/lightly-ai-selection-api-openapi.yml
- filename: lightly-ai-tags-api-openapi.yml
  format: yaml
  label: Lightly Tags API
  slug: lightly-ai-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightly-ai/refs/heads/main/openapi/lightly-ai-tags-api-openapi.yml
description: ''
domains:
- caa:
  - cdn.webflow.com.
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: lightly.ai
  spf: false
hosts:
- cert_expires: Aug 16 22:43:21 2026 GMT
  host: www.lightly.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 06:58:24 2026 GMT
  host: docs.lightly.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 16:57:30 2026 GMT
  host: api.lightly.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lightly Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lightly, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=quarantine).'
provider_name: Lightly
provider_slug: lightly-ai
slug: lightly-ai-domain-security
source_filename: lightly-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lightly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 22:43:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.lightly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 06:58:24 2026 GMT\n  hsts: false\n- host: api.lightly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 16:57:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lightly.ai\n  dnssec: true\n  caa:\n  - cdn.webflow.com.\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightly-ai/refs/heads/main/security/lightly-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Computer-Vision
- Data Curation
- Active Learning
- Embeddings
---
