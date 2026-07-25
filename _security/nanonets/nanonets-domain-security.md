---
api_specs:
- filename: nanonets-external-integrations-api-openapi.yml
  format: yaml
  label: Nanonets External Integrations API
  slug: nanonets-external-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-external-integrations-api-openapi.yml
- filename: nanonets-file-assignment-api-openapi.yml
  format: yaml
  label: Nanonets File Assignment API
  slug: nanonets-file-assignment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-file-assignment-api-openapi.yml
- filename: nanonets-file-delete-api-openapi.yml
  format: yaml
  label: Nanonets File Delete API
  slug: nanonets-file-delete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-file-delete-api-openapi.yml
- filename: nanonets-file-export-api-openapi.yml
  format: yaml
  label: Nanonets File Export API
  slug: nanonets-file-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-file-export-api-openapi.yml
- filename: nanonets-file-review-api-openapi.yml
  format: yaml
  label: Nanonets File Review API
  slug: nanonets-file-review-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-file-review-api-openapi.yml
- filename: nanonets-file-update-api-openapi.yml
  format: yaml
  label: Nanonets File Update API
  slug: nanonets-file-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-file-update-api-openapi.yml
- filename: nanonets-image-classification-predict-api-openapi.yml
  format: yaml
  label: Nanonets Image Classification Predict API
  slug: nanonets-image-classification-predict-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-image-classification-predict-api-openapi.yml
- filename: nanonets-ocr-predict-api-openapi.yml
  format: yaml
  label: Nanonets OCR Predict API
  slug: nanonets-ocr-predict-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-ocr-predict-api-openapi.yml
- filename: nanonets-ocr-retrieve-api-openapi.yml
  format: yaml
  label: Nanonets OCR Retrieve API
  slug: nanonets-ocr-retrieve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-ocr-retrieve-api-openapi.yml
- filename: nanonets-ocr-train-api-openapi.yml
  format: yaml
  label: Nanonets OCR Train API
  slug: nanonets-ocr-train-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-ocr-train-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: nanonets.com
  spf: true
hosts:
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: nanonets.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 12:29:04 2026 GMT
  host: docs.nanonets.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: app.nanonets.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nanonets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nanonets, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Nanonets
provider_slug: nanonets
slug: nanonets-domain-security
source_filename: nanonets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nanonets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.nanonets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 12:29:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.nanonets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: nanonets.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/security/nanonets-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Artificial Intelligence
- OCR
- Document AI
- Intelligent Document Processing
- Data Extraction
- Workflow Automation
- Computer Vision
- No-Code
---
