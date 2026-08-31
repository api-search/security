---
api_specs:
- filename: pdf-monkey-authentication-api-openapi.yml
  format: yaml
  label: PDF Monkey Authentication API
  slug: pdf-monkey-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-monkey/refs/heads/main/openapi/pdf-monkey-authentication-api-openapi.yml
- filename: pdf-monkey-documents-api-openapi.yml
  format: yaml
  label: PDF Monkey Documents API
  slug: pdf-monkey-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-monkey/refs/heads/main/openapi/pdf-monkey-documents-api-openapi.yml
- filename: pdf-monkey-templates-api-openapi.yml
  format: yaml
  label: PDF Monkey Templates API
  slug: pdf-monkey-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-monkey/refs/heads/main/openapi/pdf-monkey-templates-api-openapi.yml
- filename: pdf-monkey-document-cards-api-openapi.yml
  format: yaml
  label: PDF Monkey Document Cards API
  slug: pdf-monkey-document-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-monkey/refs/heads/main/openapi/pdf-monkey-document-cards-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pdfmonkey.io
  spf: true
hosts:
- cert_expires: Aug 24 20:26:14 2026 GMT
  host: www.pdfmonkey.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 22:54:23 2026 GMT
  host: pdfmonkey.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 09:41:09 2026 GMT
  host: api.pdfmonkey.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pdf Monkey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PDF Monkey, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PDF Monkey
provider_slug: pdf-monkey
slug: pdf-monkey-domain-security
source_filename: pdf-monkey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pdfmonkey.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 20:26:14 2026 GMT\n  hsts: false\n- host: pdfmonkey.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 22:54:23 2026 GMT\n  hsts: false\n- host: api.pdfmonkey.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 09:41:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pdfmonkey.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pdf-monkey/refs/heads/main/security/pdf-monkey-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- PDF
- Document Generation
- Templates
- Handlebars
- REST API
- Webhook
---
