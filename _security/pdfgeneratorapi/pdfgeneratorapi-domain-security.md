---
api_specs:
- filename: pdfgeneratorapi-openapi.yml
  format: yaml
  label: PDF Generator API Templates API
  slug: pdfgeneratorapi-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfgeneratorapi/refs/heads/main/openapi/pdfgeneratorapi-openapi.yml
- filename: pdfgeneratorapi-openapi.yml
  format: yaml
  label: PDF Generator API Documents / Generate API
  slug: pdfgeneratorapi-documents-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfgeneratorapi/refs/heads/main/openapi/pdfgeneratorapi-openapi.yml
- filename: pdfgeneratorapi-openapi.yml
  format: yaml
  label: PDF Generator API Workspaces API
  slug: pdfgeneratorapi-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfgeneratorapi/refs/heads/main/openapi/pdfgeneratorapi-openapi.yml
- filename: pdfgeneratorapi-openapi.yml
  format: yaml
  label: PDF Generator API Data Fields API
  slug: pdfgeneratorapi-data-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfgeneratorapi/refs/heads/main/openapi/pdfgeneratorapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pdfgeneratorapi.com
  spf: true
hosts:
- cert_expires: Oct  2 23:25:42 2026 GMT
  host: pdfgeneratorapi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: docs.pdfgeneratorapi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: us1.pdfgeneratorapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pdfgeneratorapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PDF Generator API, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PDF Generator API
provider_slug: pdfgeneratorapi
slug: pdfgeneratorapi-domain-security
source_filename: pdfgeneratorapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pdfgeneratorapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:25:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.pdfgeneratorapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: us1.pdfgeneratorapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: pdfgeneratorapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pdfgeneratorapi/refs/heads/main/security/pdfgeneratorapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- PDF
- Document Generation
- Templates
- Reporting
- Workspaces
---
