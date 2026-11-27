---
anonymous_access: false
api_key_in: []
api_specs:
- filename: neurobird-com-admin-api-openapi.yml
  format: yaml
  label: Neurobird Admin API
  slug: neurobird-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-admin-api-openapi.yml
- filename: neurobird-com-analyze-api-openapi.yml
  format: yaml
  label: Neurobird Analyze API
  slug: neurobird-com-analyze-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-analyze-api-openapi.yml
- filename: neurobird-com-aurora-api-openapi.yml
  format: yaml
  label: Neurobird Aurora API
  slug: neurobird-com-aurora-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-aurora-api-openapi.yml
- filename: neurobird-com-auth-api-openapi.yml
  format: yaml
  label: Neurobird Auth API
  slug: neurobird-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-auth-api-openapi.yml
- filename: neurobird-com-billing-api-openapi.yml
  format: yaml
  label: Neurobird Billing API
  slug: neurobird-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-billing-api-openapi.yml
- filename: neurobird-com-contact-api-openapi.yml
  format: yaml
  label: Neurobird Contact API
  slug: neurobird-com-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-contact-api-openapi.yml
- filename: neurobird-com-dashboard-api-openapi.yml
  format: yaml
  label: Neurobird Dashboard API
  slug: neurobird-com-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-dashboard-api-openapi.yml
- filename: neurobird-com-dashboard-html-api-openapi.yml
  format: yaml
  label: Neurobird Dashboard.html API
  slug: neurobird-com-dashboard-html-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-dashboard-html-api-openapi.yml
- filename: neurobird-com-download-api-openapi.yml
  format: yaml
  label: Neurobird Download API
  slug: neurobird-com-download-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-download-api-openapi.yml
- filename: neurobird-com-files-preview-api-openapi.yml
  format: yaml
  label: Neurobird Files Preview API
  slug: neurobird-com-files-preview-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-files-preview-api-openapi.yml
- filename: neurobird-com-generate-files-api-openapi.yml
  format: yaml
  label: Neurobird Generate Files API
  slug: neurobird-com-generate-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-generate-files-api-openapi.yml
- filename: neurobird-com-guest-usage-api-openapi.yml
  format: yaml
  label: Neurobird Guest Usage API
  slug: neurobird-com-guest-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-guest-usage-api-openapi.yml
- filename: neurobird-com-result-api-openapi.yml
  format: yaml
  label: Neurobird Result API
  slug: neurobird-com-result-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-result-api-openapi.yml
- filename: neurobird-com-screenshot-api-openapi.yml
  format: yaml
  label: Neurobird Screenshot API
  slug: neurobird-com-screenshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-screenshot-api-openapi.yml
- filename: neurobird-com-stats-api-openapi.yml
  format: yaml
  label: Neurobird Stats API
  slug: neurobird-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-stats-api-openapi.yml
- filename: neurobird-com-status-api-openapi.yml
  format: yaml
  label: Neurobird Status API
  slug: neurobird-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-status-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Neurobird Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Neurobird secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Neurobird
provider_slug: neurobird-com
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 0
    tokenUrl: /api/auth/jwt/login
  name: OAuth2PasswordBearer
  sources:
  - openapi/geo-neurobird-openapi.json
  type: oauth2
slug: neurobird-com-authentication
source_filename: neurobird-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/geo-neurobird-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: OAuth2PasswordBearer\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: /api/auth/jwt/login\n    scopes: 0\n  sources:\n  - openapi/geo-neurobird-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/neurobird-com/authentication/neurobird-com-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Artificial Intelligence
- Agency
- Product Studio
- Machine Learning
- Automation
- Consulting
---
