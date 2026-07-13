---
api_specs:
- filename: pdfmonkey-openapi.yml
  format: yaml
  label: PDFMonkey Documents API
  slug: documents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfmonkey/refs/heads/main/openapi/pdfmonkey-openapi.yml
- filename: pdfmonkey-openapi.yml
  format: yaml
  label: PDFMonkey Document Cards API
  slug: document-cards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfmonkey/refs/heads/main/openapi/pdfmonkey-openapi.yml
- filename: pdfmonkey-openapi.yml
  format: yaml
  label: PDFMonkey Templates API
  slug: templates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfmonkey/refs/heads/main/openapi/pdfmonkey-openapi.yml
- filename: pdfmonkey-openapi.yml
  format: yaml
  label: PDFMonkey Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfmonkey/refs/heads/main/openapi/pdfmonkey-openapi.yml
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
- cert_expires: Sep  3 10:10:07 2026 GMT
  host: docs.pdfmonkey.io
  hsts: true
  hsts_max_age: 315360000
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
name: Pdfmonkey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PDFMonkey, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PDFMonkey
provider_slug: pdfmonkey
slug: pdfmonkey-domain-security
source_filename: pdfmonkey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pdfmonkey.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 20:26:14 2026 GMT\n  hsts: false\n- host: docs.pdfmonkey.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 10:10:07 2026 GMT\n  hsts: true\n  hsts_max_age: 315360000\n- host: api.pdfmonkey.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 09:41:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pdfmonkey.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pdfmonkey/refs/heads/main/security/pdfmonkey-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- PDF
- Document Generation
- Templates
- HTML to PDF
- Documents
---
