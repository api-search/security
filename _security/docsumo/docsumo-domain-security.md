---
api_specs:
- filename: docsumo-openapi.yml
  format: yaml
  label: Docsumo Documents & Extraction API
  slug: docsumo-documents-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docsumo/refs/heads/main/openapi/docsumo-openapi.yml
- filename: docsumo-openapi.yml
  format: yaml
  label: Docsumo Document Types API
  slug: docsumo-document-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docsumo/refs/heads/main/openapi/docsumo-openapi.yml
- filename: docsumo-openapi.yml
  format: yaml
  label: Docsumo Review & Validation API
  slug: docsumo-review-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docsumo/refs/heads/main/openapi/docsumo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: docsumo.com
  spf: true
hosts:
- cert_expires: Aug 24 17:45:01 2026 GMT
  host: www.docsumo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 09:57:44 2026 GMT
  host: support.docsumo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 03:44:01 2026 GMT
  host: app.docsumo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Docsumo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Docsumo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Docsumo
provider_slug: docsumo
slug: docsumo-domain-security
source_filename: docsumo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.docsumo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 17:45:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.docsumo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:57:44 2026 GMT\n  hsts: null\n- host: app.docsumo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 03:44:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: docsumo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docsumo/refs/heads/main/security/docsumo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Document Processing
- IDP
- OCR
- Data Extraction
- AI
---
