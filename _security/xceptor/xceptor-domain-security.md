---
api_specs:
- filename: openapi.json
  format: json
  label: Xceptor REST API
  slug: xceptor-rest-api
  spec_type: OpenAPI
  url: https://api.xceptor.com/v1/openapi.json
- filename: workflows
  format: yaml
  label: Xceptor Workflow API
  slug: xceptor-workflow-api
  spec_type: Postman
  url: https://www.postman.com/xceptor/workspace/workflows
- filename: xceptor-document-upload-api-openapi.yml
  format: yaml
  label: Xceptor Document Upload API
  slug: xceptor-document-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/openapi/xceptor-document-upload-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: xceptor.com
  spf: true
hosts:
- host: portal.xceptor.com
  https: false
- cert_expires: Sep 25 13:17:58 2026 GMT
  host: www.xceptor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.xceptor.com
  https: false
kind: domain-security
layout: security
method: probed
name: Xceptor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xceptor, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Xceptor
provider_slug: xceptor
slug: xceptor-domain-security
source_filename: xceptor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.xceptor.com\n  https: false\n- host: www.xceptor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 13:17:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.xceptor.com\n  https: false\ndomains:\n- domain: xceptor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/security/xceptor-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- API Integration
- Data Automation
- Data Extraction
- Document Processing
- ETL
- Financial Data
- Financial Services
- Intelligent Document Processing
- Reconciliations
- Trade Operations
---
