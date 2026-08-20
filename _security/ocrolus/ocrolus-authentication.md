---
api_key_in: []
api_specs:
- filename: ocrolus-book-commands-api-openapi.yml
  format: yaml
  label: Ocrolus Book Commands API
  slug: ocrolus-book-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocrolus/refs/heads/main/openapi/ocrolus-book-commands-api-openapi.yml
- filename: ocrolus-book-queries-api-openapi.yml
  format: yaml
  label: Ocrolus Book Queries API
  slug: ocrolus-book-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocrolus/refs/heads/main/openapi/ocrolus-book-queries-api-openapi.yml
- filename: ocrolus-business-history-api-openapi.yml
  format: yaml
  label: Ocrolus Business history API
  slug: ocrolus-business-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocrolus/refs/heads/main/openapi/ocrolus-business-history-api-openapi.yml
- filename: ocrolus-business-verification-deprecated-api-openapi.yml
  format: yaml
  label: Ocrolus Business Verification (Deprecated) API
  slug: ocrolus-business-verification-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocrolus/refs/heads/main/openapi/ocrolus-business-verification-deprecated-api-openapi.yml
- filename: ocrolus-capture-api-openapi.yml
  format: yaml
  label: Ocrolus Capture API
  slug: ocrolus-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocrolus/refs/heads/main/openapi/ocrolus-capture-api-openapi.yml
- filename: ocrolus-cash-flow-analytics-api-openapi.yml
  format: yaml
  label: Ocrolus Cash Flow Analytics API
  slug: ocrolus-cash-flow-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocrolus/refs/heads/main/openapi/ocrolus-cash-flow-analytics-api-openapi.yml
- filename: ocrolus-detect-api-openapi.yml
  format: yaml
  label: Ocrolus Detect API
  slug: ocrolus-detect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocrolus/refs/heads/main/openapi/ocrolus-detect-api-openapi.yml
- filename: ocrolus-encore-api-openapi.yml
  format: yaml
  label: Ocrolus Encore API
  slug: ocrolus-encore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocrolus/refs/heads/main/openapi/ocrolus-encore-api-openapi.yml
- filename: ocrolus-file-uploads-api-openapi.yml
  format: yaml
  label: Ocrolus File Uploads API
  slug: ocrolus-file-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocrolus/refs/heads/main/openapi/ocrolus-file-uploads-api-openapi.yml
- filename: ocrolus-income-api-openapi.yml
  format: yaml
  label: Ocrolus Income API
  slug: ocrolus-income-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocrolus/refs/heads/main/openapi/ocrolus-income-api-openapi.yml
- filename: ocrolus-legacy-cash-flow-analytics-deprecated-api-openapi.yml
  format: yaml
  label: Ocrolus Legacy Cash Flow Analytics (Deprecated) API
  slug: ocrolus-legacy-cash-flow-analytics-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocrolus/refs/heads/main/openapi/ocrolus-legacy-cash-flow-analytics-deprecated-api-openapi.yml
- filename: ocrolus-oauth-api-openapi.yml
  format: yaml
  label: Ocrolus Oauth API
  slug: ocrolus-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocrolus/refs/heads/main/openapi/ocrolus-oauth-api-openapi.yml
- filename: ocrolus-org-level-webhooks-api-openapi.yml
  format: yaml
  label: Ocrolus Org Level Webhooks API
  slug: ocrolus-org-level-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocrolus/refs/heads/main/openapi/ocrolus-org-level-webhooks-api-openapi.yml
- filename: ocrolus-tag-management-api-openapi.yml
  format: yaml
  label: Ocrolus Tag Management API
  slug: ocrolus-tag-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocrolus/refs/heads/main/openapi/ocrolus-tag-management-api-openapi.yml
- filename: ocrolus-user-management-api-openapi.yml
  format: yaml
  label: Ocrolus User management API
  slug: ocrolus-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocrolus/refs/heads/main/openapi/ocrolus-user-management-api-openapi.yml
- filename: ocrolus-webhooks-api-openapi.yml
  format: yaml
  label: Ocrolus Webhooks API
  slug: ocrolus-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocrolus/refs/heads/main/openapi/ocrolus-webhooks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ocrolus Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Ocrolus secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Ocrolus
provider_slug: ocrolus
scheme_count: 1
schemes:
- description: OAuth 2.0 support via client credentials flow. See [here](doc:using-api-credentials) for usage information.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.ocrolus.com/oauth/token
  name: oauth
  sources:
  - openapi/ocrolus-account-level-webhooks-openapi.json
  - openapi/ocrolus-analyze-openapi.json
  - openapi/ocrolus-book-commands-openapi.json
  - openapi/ocrolus-book-queries-openapi.json
  - openapi/ocrolus-business-history-openapi.json
  - openapi/ocrolus-capture-openapi.json
  - openapi/ocrolus-detect-openapi.json
  - openapi/ocrolus-encore-openapi.json
  - openapi/ocrolus-file-uploads-openapi.json
  - openapi/ocrolus-income-openapi.json
  - openapi/ocrolus-org-level-webhooks-openapi.json
  - openapi/ocrolus-tag-management-openapi.json
  - openapi/ocrolus-user-management-openapi.json
  type: oauth2
slug: ocrolus-authentication
source_filename: ocrolus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/ocrolus-account-level-webhooks-openapi.json, openapi/ocrolus-analyze-openapi.json,\n  openapi/ocrolus-book-commands-openapi.json, openapi/ocrolus-book-queries-openapi.json, openapi/ocrolus-business-history-openapi.json,\n  openapi/ocrolus-capture-openapi.json, openapi/ocrolus-detect-openapi.json, openapi/ocrolus-encore-openapi.json,\n  openapi/ocrolus-file-uploads-openapi.json, openapi/ocrolus-income-openapi.json, openapi/ocrolus-org-level-webhooks-openapi.json,\n  openapi/ocrolus-tag-management-openapi.json ...\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.ocrolus.com/oauth/token\n    scopes: 0\n  description: OAuth 2.0 support via client credentials flow. See [here](doc:using-api-credentials)\n    for usage information.\n  sources:\n  - openapi/ocrolus-account-level-webhooks-openapi.json\n\
  \  - openapi/ocrolus-analyze-openapi.json\n  - openapi/ocrolus-book-commands-openapi.json\n  - openapi/ocrolus-book-queries-openapi.json\n  - openapi/ocrolus-business-history-openapi.json\n  - openapi/ocrolus-capture-openapi.json\n  - openapi/ocrolus-detect-openapi.json\n  - openapi/ocrolus-encore-openapi.json\n  - openapi/ocrolus-file-uploads-openapi.json\n  - openapi/ocrolus-income-openapi.json\n  - openapi/ocrolus-org-level-webhooks-openapi.json\n  - openapi/ocrolus-tag-management-openapi.json\n  - openapi/ocrolus-user-management-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ocrolus/refs/heads/main/authentication/ocrolus-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fintech
- Document Automation
- Lending
- Underwriting
- OCR
- Fraud Detection
- Income Verification
- Bank Statement Analysis
- Mortgage
- Machine-Learning
- Cash Flow Analytics
---
