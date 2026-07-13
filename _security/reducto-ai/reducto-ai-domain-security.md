---
api_specs:
- filename: reducto-parse-api-openapi.yml
  format: yaml
  label: Reducto Parse API
  slug: reducto-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-parse-api-openapi.yml
- filename: reducto-extract-api-openapi.yml
  format: yaml
  label: Reducto Extract API
  slug: reducto-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-extract-api-openapi.yml
- filename: reducto-split-api-openapi.yml
  format: yaml
  label: Reducto Split API
  slug: reducto-split-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-split-api-openapi.yml
- filename: reducto-edit-api-openapi.yml
  format: yaml
  label: Reducto Edit API
  slug: reducto-edit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-edit-api-openapi.yml
- filename: reducto-pipeline-api-openapi.yml
  format: yaml
  label: Reducto Pipeline API
  slug: reducto-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-pipeline-api-openapi.yml
- filename: reducto-classify-api-openapi.yml
  format: yaml
  label: Reducto Classify API
  slug: reducto-classify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-classify-api-openapi.yml
- filename: reducto-jobs-api-openapi.yml
  format: yaml
  label: Reducto Jobs API
  slug: reducto-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-jobs-api-openapi.yml
- filename: reducto-upload-api-openapi.yml
  format: yaml
  label: Reducto Upload API
  slug: reducto-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-upload-api-openapi.yml
- filename: reducto-webhooks-api-openapi.yml
  format: yaml
  label: Reducto Webhooks API
  slug: reducto-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-webhooks-api-openapi.yml
- filename: reducto-platform-api-openapi.yml
  format: yaml
  label: Reducto Platform API
  slug: reducto-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-platform-api-openapi.yml
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
