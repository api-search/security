---
api_specs:
- filename: pdf-co-openapi.yml
  format: yaml
  label: PDF.co Extraction API
  slug: pdf-co-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-co/refs/heads/main/openapi/pdf-co-openapi.yml
- filename: pdf-co-openapi.yml
  format: yaml
  label: PDF.co Conversion API
  slug: pdf-co-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-co/refs/heads/main/openapi/pdf-co-openapi.yml
- filename: pdf-co-openapi.yml
  format: yaml
  label: PDF.co Editing API
  slug: pdf-co-editing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-co/refs/heads/main/openapi/pdf-co-openapi.yml
- filename: pdf-co-openapi.yml
  format: yaml
  label: PDF.co Merging and Splitting API
  slug: pdf-co-merging-splitting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-co/refs/heads/main/openapi/pdf-co-openapi.yml
- filename: pdf-co-openapi.yml
  format: yaml
  label: PDF.co Find and Search API
  slug: pdf-co-find-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-co/refs/heads/main/openapi/pdf-co-openapi.yml
- filename: pdf-co-openapi.yml
  format: yaml
  label: PDF.co Forms API
  slug: pdf-co-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-co/refs/heads/main/openapi/pdf-co-openapi.yml
- filename: pdf-co-openapi.yml
  format: yaml
  label: PDF.co Pages API
  slug: pdf-co-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-co/refs/heads/main/openapi/pdf-co-openapi.yml
- filename: pdf-co-openapi.yml
  format: yaml
  label: PDF.co Barcodes API
  slug: pdf-co-barcodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-co/refs/heads/main/openapi/pdf-co-openapi.yml
- filename: pdf-co-openapi.yml
  format: yaml
  label: PDF.co Document, File, and System API
  slug: pdf-co-document-file-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-co/refs/heads/main/openapi/pdf-co-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pdf.co
  spf: true
hosts:
- cert_expires: Aug 31 16:09:01 2026 GMT
  host: pdf.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: docs.pdf.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: api.pdf.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pdf Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PDF.co, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PDF.co
provider_slug: pdf-co
slug: pdf-co-domain-security
source_filename: pdf-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pdf.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 16:09:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.pdf.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.pdf.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: pdf.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pdf-co/refs/heads/main/security/pdf-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- PDF
- Document Automation
- AI
- OCR
- Invoice Parsing
- Document Parsing
- Conversion
- Forms
- Barcodes
- E-Signature
---
