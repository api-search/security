---
api_specs:
- filename: mathpix-image-ocr-api-openapi.yml
  format: yaml
  label: Mathpix Image OCR API
  slug: mathpix-image-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-image-ocr-api-openapi.yml
- filename: mathpix-document-ocr-api-openapi.yml
  format: yaml
  label: Mathpix Document OCR API
  slug: mathpix-document-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-document-ocr-api-openapi.yml
- filename: mathpix-convert-api-openapi.yml
  format: yaml
  label: Mathpix Convert API
  slug: mathpix-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-convert-api-openapi.yml
- filename: mathpix-batch-api-openapi.yml
  format: yaml
  label: Mathpix Batch API
  slug: mathpix-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-batch-api-openapi.yml
- filename: mathpix-strokes-api-openapi.yml
  format: yaml
  label: Mathpix Strokes API
  slug: mathpix-strokes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-strokes-api-openapi.yml
- filename: mathpix-app-tokens-api-openapi.yml
  format: yaml
  label: Mathpix App Tokens API
  slug: mathpix-app-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-app-tokens-api-openapi.yml
- filename: mathpix-ocr-usage-api-openapi.yml
  format: yaml
  label: Mathpix OCR Usage API
  slug: mathpix-ocr-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-ocr-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mathpix.com
  spf: true
hosts:
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: docs.mathpix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: api.mathpix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mathpix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mathpix, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mathpix
provider_slug: mathpix
slug: mathpix-domain-security
source_filename: mathpix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.mathpix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: false\n- host: api.mathpix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: mathpix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/security/mathpix-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- OCR
- STEM
- Math
- Chemistry
- Document Conversion
- PDF
- LaTeX
- Handwriting
- AI
- Machine Learning
---
