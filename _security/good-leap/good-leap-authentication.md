---
api_key_in: []
api_specs:
- filename: good-leap-authorization-elevation-management-api-openapi.yml
  format: yaml
  label: Good Leap Authorization & Elevation Management API
  slug: good-leap-authorization-elevation-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/openapi/good-leap-authorization-elevation-management-api-openapi.yml
- filename: good-leap-calculate-payments-api-openapi.yml
  format: yaml
  label: Good Leap Calculate Payments API
  slug: good-leap-calculate-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/openapi/good-leap-calculate-payments-api-openapi.yml
- filename: good-leap-case-loan-stipulations-management-api-openapi.yml
  format: yaml
  label: Good Leap Case (loan stipulations) Management API
  slug: good-leap-case-loan-stipulations-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/openapi/good-leap-case-loan-stipulations-management-api-openapi.yml
- filename: good-leap-disclosures-api-openapi.yml
  format: yaml
  label: Good Leap Disclosures API
  slug: good-leap-disclosures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/openapi/good-leap-disclosures-api-openapi.yml
- filename: good-leap-install-categories-loan-limitations-api-openapi.yml
  format: yaml
  label: Good Leap Install Categories & Loan Limitations API
  slug: good-leap-install-categories-loan-limitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/openapi/good-leap-install-categories-loan-limitations-api-openapi.yml
- filename: good-leap-loan-change-orders-api-openapi.yml
  format: yaml
  label: Good Leap Loan Change Orders API
  slug: good-leap-loan-change-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/openapi/good-leap-loan-change-orders-api-openapi.yml
- filename: good-leap-loan-documents-management-api-openapi.yml
  format: yaml
  label: Good Leap Loan Documents Management API
  slug: good-leap-loan-documents-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/openapi/good-leap-loan-documents-management-api-openapi.yml
- filename: good-leap-loan-notes-management-api-openapi.yml
  format: yaml
  label: Good Leap Loan Notes Management API
  slug: good-leap-loan-notes-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/openapi/good-leap-loan-notes-management-api-openapi.yml
- filename: good-leap-loan-status-api-openapi.yml
  format: yaml
  label: Good Leap Loan Status API
  slug: good-leap-loan-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/openapi/good-leap-loan-status-api-openapi.yml
- filename: good-leap-loan-submission-api-openapi.yml
  format: yaml
  label: Good Leap Loan Submission API
  slug: good-leap-loan-submission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/openapi/good-leap-loan-submission-api-openapi.yml
- filename: good-leap-loan-tag-management-api-openapi.yml
  format: yaml
  label: Good Leap Loan Tag Management API
  slug: good-leap-loan-tag-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/openapi/good-leap-loan-tag-management-api-openapi.yml
- filename: good-leap-milestone-management-api-openapi.yml
  format: yaml
  label: Good Leap Milestone Management API
  slug: good-leap-milestone-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/openapi/good-leap-milestone-management-api-openapi.yml
- filename: good-leap-project-management-api-openapi.yml
  format: yaml
  label: Good Leap Project Management API
  slug: good-leap-project-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/openapi/good-leap-project-management-api-openapi.yml
- filename: good-leap-promotions-api-openapi.yml
  format: yaml
  label: Good Leap Promotions API
  slug: good-leap-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/openapi/good-leap-promotions-api-openapi.yml
- filename: good-leap-states-channels-api-openapi.yml
  format: yaml
  label: Good Leap States & Channels API
  slug: good-leap-states-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/openapi/good-leap-states-channels-api-openapi.yml
- filename: good-leap-toolbox-api-openapi.yml
  format: yaml
  label: Good Leap Toolbox API
  slug: good-leap-toolbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/openapi/good-leap-toolbox-api-openapi.yml
- filename: good-leap-user-management-api-openapi.yml
  format: yaml
  label: Good Leap User Management API
  slug: good-leap-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/openapi/good-leap-user-management-api-openapi.yml
- filename: good-leap-verify-loan-details-api-openapi.yml
  format: yaml
  label: Good Leap Verify Loan Details API
  slug: good-leap-verify-loan-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/openapi/good-leap-verify-loan-details-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Good Leap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Good Leap secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Good Leap
provider_slug: good-leap
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT obtained via POST /posfinancing/rest/v2/auth/token (organizationId), refreshed via /auth/token/refresh.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/good-leap-developer-api-openapi.yml
  type: http
slug: good-leap-authentication
source_filename: good-leap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/good-leap-developer-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT obtained via POST /posfinancing/rest/v2/auth/token (organizationId), refreshed\n    via /auth/token/refresh.\n  sources:\n  - openapi/good-leap-developer-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/good-leap/refs/heads/main/authentication/good-leap-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Financing
- Lending
- Solar
- Home Improvement
- Sustainability
- Point of Sale
- Loans
- Payments
---
