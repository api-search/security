---
api_key_in: []
api_specs:
- filename: vantage-sh-openapi.yml
  format: yaml
  label: Vantage Costs API
  slug: vantage-sh-costs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage-sh/refs/heads/main/openapi/vantage-sh-openapi.yml
- filename: vantage-sh-openapi.yml
  format: yaml
  label: Vantage Cost Reports API
  slug: vantage-sh-cost-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage-sh/refs/heads/main/openapi/vantage-sh-openapi.yml
- filename: vantage-sh-openapi.yml
  format: yaml
  label: Vantage Resources API
  slug: vantage-sh-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage-sh/refs/heads/main/openapi/vantage-sh-openapi.yml
- filename: vantage-sh-openapi.yml
  format: yaml
  label: Vantage Recommendations API
  slug: vantage-sh-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage-sh/refs/heads/main/openapi/vantage-sh-openapi.yml
- filename: vantage-sh-openapi.yml
  format: yaml
  label: Vantage Budgets API
  slug: vantage-sh-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage-sh/refs/heads/main/openapi/vantage-sh-openapi.yml
- filename: vantage-sh-openapi.yml
  format: yaml
  label: Vantage Cost Alerts API
  slug: vantage-sh-cost-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage-sh/refs/heads/main/openapi/vantage-sh-openapi.yml
- filename: vantage-sh-openapi.yml
  format: yaml
  label: Vantage Anomaly Alerts API
  slug: vantage-sh-anomaly-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage-sh/refs/heads/main/openapi/vantage-sh-openapi.yml
- filename: vantage-sh-openapi.yml
  format: yaml
  label: Vantage Segments API
  slug: vantage-sh-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage-sh/refs/heads/main/openapi/vantage-sh-openapi.yml
- filename: vantage-sh-openapi.yml
  format: yaml
  label: Vantage Financial Commitments API
  slug: vantage-sh-financial-commitments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage-sh/refs/heads/main/openapi/vantage-sh-openapi.yml
- filename: vantage-sh-openapi.yml
  format: yaml
  label: Vantage Dashboards API
  slug: vantage-sh-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage-sh/refs/heads/main/openapi/vantage-sh-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Vantage Sh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vantage secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vantage
provider_slug: vantage-sh
scheme_count: 1
schemes:
- description: 'Vantage authenticates with an OAuth2 client-credentials bearer token. Generate or copy a token from the Vantage console under Account / Profile (console.vantage.sh/account/profile) and pass it as `Authorization: Bearer YOUR_API_TOKEN`. Tokens carry read and/or write scopes.'
  flow: clientCredentials
  name: oauth2
  scopes:
    read: Grants read access
    write: Grants write access
  sources:
  - openapi/vantage-sh-openapi.yml
  - https://vantage.readme.io/reference/authentication
  tokenUrl: https://console.vantage.sh/account/profile
  type: oauth2
slug: vantage-sh-authentication
source_filename: vantage-sh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vantage-sh-openapi.yml\nsummary:\n  types:\n  - oauth2\nschemes:\n- name: oauth2\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://console.vantage.sh/account/profile\n  scopes:\n    read: Grants read access\n    write: Grants write access\n  description: 'Vantage authenticates with an OAuth2 client-credentials bearer token.\n    Generate or copy a token from the Vantage console under Account / Profile\n    (console.vantage.sh/account/profile) and pass it as `Authorization: Bearer\n    YOUR_API_TOKEN`. Tokens carry read and/or write scopes.'\n  sources:\n  - openapi/vantage-sh-openapi.yml\n  - https://vantage.readme.io/reference/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vantage-sh/refs/heads/main/authentication/vantage-sh-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Cloud Cost
- FinOps
- Cost Management
- Cloud Optimization
- Cost Visibility
- Cloud Spend
- Multi-Cloud
---
