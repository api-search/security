---
api_specs:
- filename: zuva-openapi.yml
  format: yaml
  label: Zuva Files API
  slug: files
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-openapi.yml
- filename: zuva-openapi.yml
  format: yaml
  label: Zuva Field Extraction API
  slug: field-extraction
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-openapi.yml
- filename: zuva-openapi.yml
  format: yaml
  label: Zuva Classification API
  slug: classification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-openapi.yml
- filename: zuva-openapi.yml
  format: yaml
  label: Zuva Language API
  slug: language
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-openapi.yml
- filename: zuva-openapi.yml
  format: yaml
  label: Zuva OCR API
  slug: ocr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-openapi.yml
- filename: zuva-openapi.yml
  format: yaml
  label: Zuva Fields Catalog API
  slug: fields-catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zuva.ai
  spf: true
hosts:
- cert_expires: Oct  8 04:45:31 2026 GMT
  host: zuva.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 14:40:20 2026 GMT
  host: us.app.zuva.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zuva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zuva, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zuva
provider_slug: zuva
slug: zuva-domain-security
source_filename: zuva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zuva.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 04:45:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: us.app.zuva.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 14:40:20 2026 GMT\n  hsts: null\ndomains:\n- domain: zuva.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/security/zuva-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Document AI
- Contract Analysis
- Field Extraction
- Classification
- OCR
---
