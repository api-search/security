---
api_specs:
- filename: workflows
  format: yaml
  label: Xceptor Workflow API
  slug: xceptor-workflow-api
  spec_type: Postman
  url: https://www.postman.com/xceptor/workspace/workflows
- filename: xceptor-authentication-api-openapi.yml
  format: yaml
  label: Xceptor Authentication API
  slug: xceptor-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/openapi/xceptor-authentication-api-openapi.yml
- filename: xceptor-data-sources-api-openapi.yml
  format: yaml
  label: Xceptor Data Sources API
  slug: xceptor-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/openapi/xceptor-data-sources-api-openapi.yml
- filename: xceptor-documents-api-openapi.yml
  format: yaml
  label: Xceptor Documents API
  slug: xceptor-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/openapi/xceptor-documents-api-openapi.yml
- filename: xceptor-extraction-api-openapi.yml
  format: yaml
  label: Xceptor Extraction API
  slug: xceptor-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/openapi/xceptor-extraction-api-openapi.yml
- filename: xceptor-health-api-openapi.yml
  format: yaml
  label: Xceptor Health API
  slug: xceptor-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/openapi/xceptor-health-api-openapi.yml
- filename: xceptor-jobs-api-openapi.yml
  format: yaml
  label: Xceptor Jobs API
  slug: xceptor-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/openapi/xceptor-jobs-api-openapi.yml
- filename: xceptor-templates-api-openapi.yml
  format: yaml
  label: Xceptor Templates API
  slug: xceptor-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/openapi/xceptor-templates-api-openapi.yml
- filename: xceptor-workflow-runs-api-openapi.yml
  format: yaml
  label: Xceptor Workflow Runs API
  slug: xceptor-workflow-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/openapi/xceptor-workflow-runs-api-openapi.yml
- filename: xceptor-workflow-steps-api-openapi.yml
  format: yaml
  label: Xceptor Workflow Steps API
  slug: xceptor-workflow-steps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/openapi/xceptor-workflow-steps-api-openapi.yml
- filename: xceptor-workflows-api-openapi.yml
  format: yaml
  label: Xceptor Workflows API
  slug: xceptor-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xceptor/refs/heads/main/openapi/xceptor-workflows-api-openapi.yml
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
