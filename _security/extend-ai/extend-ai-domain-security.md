---
api_specs:
- filename: extend-ai-openapi.yml
  format: yaml
  label: Extend Files API
  slug: files
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/openapi/extend-ai-openapi.yml
- filename: extend-ai-openapi.yml
  format: yaml
  label: Extend Processors API
  slug: processors
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/openapi/extend-ai-openapi.yml
- filename: extend-ai-openapi.yml
  format: yaml
  label: Extend Processor Runs API
  slug: processor-runs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/openapi/extend-ai-openapi.yml
- filename: extend-ai-openapi.yml
  format: yaml
  label: Extend Workflows API
  slug: workflows
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/openapi/extend-ai-openapi.yml
- filename: extend-ai-openapi.yml
  format: yaml
  label: Extend Workflow Runs API
  slug: workflow-runs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/openapi/extend-ai-openapi.yml
- filename: extend-ai-openapi.yml
  format: yaml
  label: Extend Evaluations API
  slug: evaluations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/openapi/extend-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: extend.ai
  spf: true
hosts:
- cert_expires: Sep  9 15:06:36 2026 GMT
  host: www.extend.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 19:40:10 2026 GMT
  host: docs.extend.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: api.extend.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Extend Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Extend, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Extend
provider_slug: extend-ai
slug: extend-ai-domain-security
source_filename: extend-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.extend.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 15:06:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.extend.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 19:40:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.extend.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: extend.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/extend-ai/refs/heads/main/security/extend-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Document Processing
- Document AI
- Intelligent Document Processing
- OCR
- Extraction
- Classification
---
