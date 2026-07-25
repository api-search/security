---
api_specs:
- filename: reducto-ai-classify-api-openapi.yml
  format: yaml
  label: reducto-ai Classify API
  slug: reducto-ai-classify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-classify-api-openapi.yml
- filename: reducto-ai-edit-api-openapi.yml
  format: yaml
  label: reducto-ai Edit API
  slug: reducto-ai-edit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-edit-api-openapi.yml
- filename: reducto-ai-extract-api-openapi.yml
  format: yaml
  label: reducto-ai Extract API
  slug: reducto-ai-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-extract-api-openapi.yml
- filename: reducto-ai-jobs-api-openapi.yml
  format: yaml
  label: reducto-ai Jobs API
  slug: reducto-ai-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-jobs-api-openapi.yml
- filename: reducto-ai-parse-api-openapi.yml
  format: yaml
  label: reducto-ai Parse API
  slug: reducto-ai-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-parse-api-openapi.yml
- filename: reducto-ai-pipeline-api-openapi.yml
  format: yaml
  label: reducto-ai Pipeline API
  slug: reducto-ai-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-pipeline-api-openapi.yml
- filename: reducto-ai-platform-api-openapi.yml
  format: yaml
  label: reducto-ai Platform API
  slug: reducto-ai-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-platform-api-openapi.yml
- filename: reducto-ai-split-api-openapi.yml
  format: yaml
  label: reducto-ai Split API
  slug: reducto-ai-split-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-split-api-openapi.yml
- filename: reducto-ai-upload-api-openapi.yml
  format: yaml
  label: reducto-ai Upload API
  slug: reducto-ai-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-upload-api-openapi.yml
- filename: reducto-ai-webhooks-api-openapi.yml
  format: yaml
  label: reducto-ai Webhooks API
  slug: reducto-ai-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reducto.ai
  spf: true
hosts:
- cert_expires: Sep  6 01:49:49 2026 GMT
  host: reducto.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 11:39:00 2026 GMT
  host: docs.reducto.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: platform.reducto.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reducto Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for reducto-ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: reducto-ai
provider_slug: reducto-ai
slug: reducto-ai-domain-security
source_filename: reducto-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reducto.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 01:49:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.reducto.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 11:39:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: platform.reducto.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: reducto.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/security/reducto-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
