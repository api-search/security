---
api_key_in: []
api_specs:
- filename: productiv-app-details-api-openapi.yml
  format: yaml
  label: Productiv App Details API
  slug: productiv-app-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-app-details-api-openapi.yml
- filename: productiv-app-summaries-api-openapi.yml
  format: yaml
  label: Productiv App Summaries API
  slug: productiv-app-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-app-summaries-api-openapi.yml
- filename: productiv-applications-api-openapi.yml
  format: yaml
  label: Productiv Applications API
  slug: productiv-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-applications-api-openapi.yml
- filename: productiv-audit-events-api-openapi.yml
  format: yaml
  label: Productiv Audit Events API
  slug: productiv-audit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-audit-events-api-openapi.yml
- filename: productiv-authentication-api-openapi.yml
  format: yaml
  label: Productiv Authentication API
  slug: productiv-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-authentication-api-openapi.yml
- filename: productiv-batch-upload-api-openapi.yml
  format: yaml
  label: Productiv Batch Upload API
  slug: productiv-batch-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-batch-upload-api-openapi.yml
- filename: productiv-org-chart-api-openapi.yml
  format: yaml
  label: Productiv Org Chart API
  slug: productiv-org-chart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-org-chart-api-openapi.yml
- filename: productiv-provisioned-users-api-openapi.yml
  format: yaml
  label: Productiv Provisioned Users API
  slug: productiv-provisioned-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-provisioned-users-api-openapi.yml
- filename: productiv-provisioning-workflows-api-openapi.yml
  format: yaml
  label: Productiv Provisioning Workflows API
  slug: productiv-provisioning-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-provisioning-workflows-api-openapi.yml
- filename: productiv-spend-data-api-openapi.yml
  format: yaml
  label: Productiv Spend Data API
  slug: productiv-spend-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-spend-data-api-openapi.yml
- filename: productiv-usage-events-api-openapi.yml
  format: yaml
  label: Productiv Usage Events API
  slug: productiv-usage-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/openapi/productiv-usage-events-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Productiv Authentication
name_suffix: Authentication
oauth_flows: []
overview: Productiv secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Productiv
provider_slug: productiv
scheme_count: 1
schemes:
- bearerFormat: OAuth2
  description: Bearer token obtained from the OAuth2 token endpoint at https://login.api.productiv.com/oauth2/token using client credentials grant type.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/productiv-developer-openapi.yml
  type: http
slug: productiv-authentication
source_filename: productiv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/productiv-developer-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2\n  description: Bearer token obtained from the OAuth2 token endpoint at https://login.api.productiv.com/oauth2/token\n    using client credentials grant type.\n  sources:\n  - openapi/productiv-developer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/authentication/productiv-authentication.yml
summary_line: http · 1 scheme
tags:
- Application Portfolio
- Provisioning
- SaaS Management
- Spend Management
- Usage Analytics
---
