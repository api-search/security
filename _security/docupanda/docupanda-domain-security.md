---
api_specs:
- filename: docupanda-analysis-api-openapi.yml
  format: yaml
  label: DocuPipe Analysis API
  slug: docupanda-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-analysis-api-openapi.yml
- filename: docupanda-account-api-openapi.yml
  format: yaml
  label: DocuPipe Account API
  slug: docupanda-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-account-api-openapi.yml
- filename: docupanda-account-api-openapi.yml
  format: yaml
  label: DocuPipe Account API
  slug: docupanda-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-account-api-openapi.yml
- filename: docupanda-analysis-api-openapi.yml
  format: yaml
  label: DocuPipe Analysis API
  slug: docupanda-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-analysis-api-openapi.yml
- filename: docupanda-classification-api-openapi.yml
  format: yaml
  label: DocuPipe Classification API
  slug: docupanda-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-classification-api-openapi.yml
- filename: docupanda-document-api-openapi.yml
  format: yaml
  label: DocuPipe Document API
  slug: docupanda-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-document-api-openapi.yml
- filename: docupanda-job-api-openapi.yml
  format: yaml
  label: DocuPipe Job API
  slug: docupanda-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-job-api-openapi.yml
- filename: docupanda-review-api-openapi.yml
  format: yaml
  label: DocuPipe Review API
  slug: docupanda-review-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-review-api-openapi.yml
- filename: docupanda-schema-api-openapi.yml
  format: yaml
  label: DocuPipe Schema API
  slug: docupanda-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-schema-api-openapi.yml
- filename: docupanda-standardization-api-openapi.yml
  format: yaml
  label: DocuPipe Standardization API
  slug: docupanda-standardization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-standardization-api-openapi.yml
- filename: docupanda-transformation-api-openapi.yml
  format: yaml
  label: DocuPipe Transformation API
  slug: docupanda-transformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-transformation-api-openapi.yml
- filename: docupanda-webhook-api-openapi.yml
  format: yaml
  label: DocuPipe Webhook API
  slug: docupanda-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-webhook-api-openapi.yml
- filename: docupanda-workflow-api-openapi.yml
  format: yaml
  label: DocuPipe Workflow API
  slug: docupanda-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/openapi/docupanda-workflow-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: docupipe.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: docupanda.io
  spf: true
hosts:
- cert_expires: Aug 13 01:14:53 2026 GMT
  host: www.docupipe.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 08:56:05 2026 GMT
  host: www.docupanda.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 14:15:40 2026 GMT
  host: docs.docupipe.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Docupanda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DocuPipe, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DocuPipe
provider_slug: docupanda
slug: docupanda-domain-security
source_filename: docupanda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.docupipe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 01:14:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.docupanda.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 08:56:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.docupipe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 14:15:40 2026 GMT\n  hsts: null\ndomains:\n- domain: docupipe.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: docupanda.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docupanda/refs/heads/main/security/docupanda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Document Extraction
- Document Intelligence
- Intelligent Document Processing
- OCR
- Document AI
---
