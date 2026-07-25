---
api_key_in: []
api_specs:
- filename: sec-company-concept-api-openapi.yml
  format: yaml
  label: SEC EDGAR Company Concept API
  slug: sec-company-concept-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-company-concept-api-openapi.yml
- filename: sec-company-facts-api-openapi.yml
  format: yaml
  label: SEC EDGAR Company Facts API
  slug: sec-company-facts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-company-facts-api-openapi.yml
- filename: sec-edgar-operational-status-api-api-openapi.yml
  format: yaml
  label: SEC EDGAR EDGAR Operational Status API API
  slug: sec-edgar-operational-status-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-edgar-operational-status-api-api-openapi.yml
- filename: sec-filer-management-api-api-openapi.yml
  format: yaml
  label: SEC EDGAR Filer Management API API
  slug: sec-filer-management-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-filer-management-api-api-openapi.yml
- filename: sec-frames-api-openapi.yml
  format: yaml
  label: SEC EDGAR Frames API
  slug: sec-frames-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-frames-api-openapi.yml
- filename: sec-search-api-openapi.yml
  format: yaml
  label: SEC EDGAR Search API
  slug: sec-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-search-api-openapi.yml
- filename: sec-submission-api-api-openapi.yml
  format: yaml
  label: SEC EDGAR Submission API API
  slug: sec-submission-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-submission-api-api-openapi.yml
- filename: sec-submission-status-api-api-openapi.yml
  format: yaml
  label: SEC EDGAR Submission Status API API
  slug: sec-submission-status-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-submission-status-api-api-openapi.yml
- filename: sec-submissions-api-openapi.yml
  format: yaml
  label: SEC EDGAR Submissions API
  slug: sec-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-submissions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sec Authentication
name_suffix: Authentication
oauth_flows: []
overview: SEC EDGAR secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SEC EDGAR
provider_slug: sec
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: A Filer API Token would be required to be presented to use any of the EDGAR APIs—the EDGAR Submission API, EDGAR Submission Status API, and EDGAR Operational Status API. A User API Token would be required to be presented for the EDGAR Submission API only. EDGAR submissions made using the EDGAR Submission API would be subject to the same authentication and validation procedures that apply to submis
  name: Filer API Token and User API Token
  scheme: bearer
  sources:
  - openapi/sec-edgar-filer-openapi.yml
  type: http
slug: sec-authentication
source_filename: sec-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sec-edgar-filer-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: Filer API Token and User API Token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: A Filer API Token would be required to be presented to use any of the EDGAR APIs—the\n    EDGAR Submission API, EDGAR Submission Status API, and EDGAR Operational Status API. A User\n    API Token would be required to be presented for the EDGAR Submission API only. EDGAR submissions\n    made using the EDGAR Submission API would be subject to the same authentication and validation\n    procedures that apply to submis\n  sources:\n  - openapi/sec-edgar-filer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/authentication/sec-authentication.yml
summary_line: http · 1 scheme
tags:
- Financial Data
- SEC
- EDGAR
- Public Company Filings
- XBRL
- Regulatory
- Government
- Financial Reporting
- Company Submissions
- Securities
---
