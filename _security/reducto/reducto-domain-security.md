---
api_specs:
- filename: reducto-cancel-api-openapi.yml
  format: yaml
  label: Reducto Cancel API
  slug: reducto-cancel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-cancel-api-openapi.yml
- filename: reducto-classify-api-openapi.yml
  format: yaml
  label: Reducto Classify API
  slug: reducto-classify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-classify-api-openapi.yml
- filename: reducto-configure-webhook-api-openapi.yml
  format: yaml
  label: Reducto Configure Webhook API
  slug: reducto-configure-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-configure-webhook-api-openapi.yml
- filename: reducto-edit-api-openapi.yml
  format: yaml
  label: Reducto Edit API
  slug: reducto-edit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-edit-api-openapi.yml
- filename: reducto-edit-async-api-openapi.yml
  format: yaml
  label: Reducto Edit Async API
  slug: reducto-edit-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-edit-async-api-openapi.yml
- filename: reducto-extract-api-openapi.yml
  format: yaml
  label: Reducto Extract API
  slug: reducto-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-extract-api-openapi.yml
- filename: reducto-extract-async-api-openapi.yml
  format: yaml
  label: Reducto Extract Async API
  slug: reducto-extract-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-extract-async-api-openapi.yml
- filename: reducto-job-api-openapi.yml
  format: yaml
  label: Reducto Job API
  slug: reducto-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-job-api-openapi.yml
- filename: reducto-jobs-api-openapi.yml
  format: yaml
  label: Reducto Jobs API
  slug: reducto-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-jobs-api-openapi.yml
- filename: reducto-parse-api-openapi.yml
  format: yaml
  label: Reducto Parse API
  slug: reducto-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-parse-api-openapi.yml
- filename: reducto-parse-async-api-openapi.yml
  format: yaml
  label: Reducto Parse Async API
  slug: reducto-parse-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-parse-async-api-openapi.yml
- filename: reducto-pipeline-api-openapi.yml
  format: yaml
  label: Reducto Pipeline API
  slug: reducto-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-pipeline-api-openapi.yml
- filename: reducto-pipeline-async-api-openapi.yml
  format: yaml
  label: Reducto Pipeline Async API
  slug: reducto-pipeline-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-pipeline-async-api-openapi.yml
- filename: reducto-split-api-openapi.yml
  format: yaml
  label: Reducto Split API
  slug: reducto-split-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-split-api-openapi.yml
- filename: reducto-split-async-api-openapi.yml
  format: yaml
  label: Reducto Split Async API
  slug: reducto-split-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-split-async-api-openapi.yml
- filename: reducto-upload-api-openapi.yml
  format: yaml
  label: Reducto Upload API
  slug: reducto-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-upload-api-openapi.yml
- filename: reducto-version-api-openapi.yml
  format: yaml
  label: Reducto Version API
  slug: reducto-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-version-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reducto.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: reductoai.com
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
- host: api.reductoai.com
  https: false
kind: domain-security
layout: security
method: probed
name: Reducto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reducto, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Reducto
provider_slug: reducto
slug: reducto-domain-security
source_filename: reducto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reducto.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 01:49:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.reducto.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 11:39:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.reductoai.com\n  https: false\ndomains:\n- domain: reducto.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: reductoai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/security/reducto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Document Parsing
- PDF
- OCR
- Data Extraction
- AI
- Machine Learning
- Document Intelligence
- Structured Data
---
