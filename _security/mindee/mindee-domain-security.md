---
api_specs:
- filename: mindee-extraction-api-openapi.yml
  format: yaml
  label: Mindee Extraction API
  slug: mindee-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindee/refs/heads/main/openapi/mindee-extraction-api-openapi.yml
- filename: mindee-classification-api-openapi.yml
  format: yaml
  label: Mindee Classification API
  slug: mindee-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindee/refs/heads/main/openapi/mindee-classification-api-openapi.yml
- filename: mindee-crop-api-openapi.yml
  format: yaml
  label: Mindee Crop API
  slug: mindee-crop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindee/refs/heads/main/openapi/mindee-crop-api-openapi.yml
- filename: mindee-ocr-api-openapi.yml
  format: yaml
  label: Mindee OCR API
  slug: mindee-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindee/refs/heads/main/openapi/mindee-ocr-api-openapi.yml
- filename: mindee-split-api-openapi.yml
  format: yaml
  label: Mindee Split API
  slug: mindee-split-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindee/refs/heads/main/openapi/mindee-split-api-openapi.yml
- filename: mindee-jobs-api-openapi.yml
  format: yaml
  label: Mindee Jobs API
  slug: mindee-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindee/refs/heads/main/openapi/mindee-jobs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mindee.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: mindee.net
  spf: true
hosts:
- cert_expires: Sep 28 14:01:19 2026 GMT
  host: mindee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 16:34:26 2026 GMT
  host: docs.mindee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 06:15:15 2026 GMT
  host: api-v2.mindee.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mindee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mindee, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mindee
provider_slug: mindee
slug: mindee-domain-security
source_filename: mindee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mindee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 14:01:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.mindee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 16:34:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-v2.mindee.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 06:15:15 2026 GMT\n  hsts: null\ndomains:\n- domain: mindee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: mindee.net\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mindee/refs/heads/main/security/mindee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Document Parsing
- OCR
- IDP
- AI
- Machine Learning
- Invoices
- Receipts
- IDs
- Computer Vision
---
