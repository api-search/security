---
api_key_in: []
api_specs:
- filename: figma-api-openapi.yml
  format: yaml
  label: Figma API
  slug: figma-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma REST API
  slug: figma-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
- filename: figma-files-api-openapi.yml
  format: yaml
  label: Figma Files API
  slug: figma-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-files-api-openapi.yml
- filename: figma-images-api-openapi.yml
  format: yaml
  label: Figma Images API
  slug: figma-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-images-api-openapi.yml
- filename: figma-teams-api-openapi.yml
  format: yaml
  label: Figma Teams API
  slug: figma-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-teams-api-openapi.yml
- filename: figma-projects-api-openapi.yml
  format: yaml
  label: Figma Projects API
  slug: figma-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-projects-api-openapi.yml
- filename: figma-me-api-openapi.yml
  format: yaml
  label: Figma Me API
  slug: figma-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-me-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma Components API
  slug: figma-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
- filename: figma-component-sets-api-openapi.yml
  format: yaml
  label: Figma Component Sets API
  slug: figma-component-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-component-sets-api-openapi.yml
- filename: figma-styles-api-openapi.yml
  format: yaml
  label: Figma Styles API
  slug: figma-styles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-styles-api-openapi.yml
- filename: figma-activity-logs-api-openapi.yml
  format: yaml
  label: Figma Activity Logs API
  slug: figma-activity-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-activity-logs-api-openapi.yml
- filename: figma-payments-api-openapi.yml
  format: yaml
  label: Figma Payments API
  slug: figma-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-payments-api-openapi.yml
- filename: figma-dev-resources-api-openapi.yml
  format: yaml
  label: Figma Dev Resources API
  slug: figma-dev-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-dev-resources-api-openapi.yml
- filename: figma-analytics-api-openapi.yml
  format: yaml
  label: Figma Analytics API
  slug: figma-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-analytics-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma Comments API
  slug: figma-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma Version History API
  slug: figma-version-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma Variables API
  slug: figma-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
- filename: figma-rest-api-openapi.yml
  format: yaml
  label: Figma Library Analytics API
  slug: figma-library-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/openapi/figma-rest-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Figma Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Figma secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Figma
provider_slug: figma
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://www.figma.com/oauth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.figma.com/v1/oauth/token
  name: OrgOAuth2
  sources:
  - openapi/figma-activity-logs-api-openapi.yml
  - openapi/figma-analytics-api-openapi.yml
  - openapi/figma-api-openapi.yml
  - openapi/figma-component-sets-api-openapi.yml
  - openapi/figma-dev-resources-api-openapi.yml
  - openapi/figma-files-api-openapi.yml
  - openapi/figma-images-api-openapi.yml
  - openapi/figma-me-api-openapi.yml
  - openapi/figma-projects-api-openapi.yml
  - openapi/figma-rest-api-openapi.yml
  - openapi/figma-styles-api-openapi.yml
  - openapi/figma-teams-api-openapi.yml
  type: oauth2
- bearerFormat: Figma Personal Access Token
  description: Personal Access Token for authentication
  name: PersonalAccessToken
  scheme: bearer
  sources:
  - openapi/figma-analytics-api-openapi.yml
  - openapi/figma-api-openapi.yml
  - openapi/figma-component-sets-api-openapi.yml
  - openapi/figma-dev-resources-api-openapi.yml
  - openapi/figma-files-api-openapi.yml
  - openapi/figma-images-api-openapi.yml
  - openapi/figma-me-api-openapi.yml
  - openapi/figma-payments-api-openapi.yml
  - openapi/figma-projects-api-openapi.yml
  - openapi/figma-rest-api-openapi.yml
  - openapi/figma-styles-api-openapi.yml
  - openapi/figma-teams-api-openapi.yml
  type: http
slug: figma-authentication
source_filename: figma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/figma-activity-logs-api-openapi.yml, openapi/figma-analytics-api-openapi.yml,\n  openapi/figma-api-openapi.yml, openapi/figma-component-sets-api-openapi.yml, openapi/figma-dev-resources-api-openapi.yml,\n  openapi/figma-files-api-openapi.yml, openapi/figma-images-api-openapi.yml, openapi/figma-me-api-openapi.yml,\n  openapi/figma-payments-api-openapi.yml, openapi/figma-projects-api-openapi.yml, openapi/figma-rest-api-openapi.yml,\n  openapi/figma-styles-api-openapi.yml ...\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OrgOAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.figma.com/oauth\n    tokenUrl: https://api.figma.com/v1/oauth/token\n    scopes: 1\n  sources:\n  - openapi/figma-activity-logs-api-openapi.yml\n  - openapi/figma-analytics-api-openapi.yml\n  - openapi/figma-api-openapi.yml\n  - openapi/figma-component-sets-api-openapi.yml\n\
  \  - openapi/figma-dev-resources-api-openapi.yml\n  - openapi/figma-files-api-openapi.yml\n  - openapi/figma-images-api-openapi.yml\n  - openapi/figma-me-api-openapi.yml\n  - openapi/figma-projects-api-openapi.yml\n  - openapi/figma-rest-api-openapi.yml\n  - openapi/figma-styles-api-openapi.yml\n  - openapi/figma-teams-api-openapi.yml\n- name: PersonalAccessToken\n  type: http\n  scheme: bearer\n  bearerFormat: Figma Personal Access Token\n  description: Personal Access Token for authentication\n  sources:\n  - openapi/figma-analytics-api-openapi.yml\n  - openapi/figma-api-openapi.yml\n  - openapi/figma-component-sets-api-openapi.yml\n  - openapi/figma-dev-resources-api-openapi.yml\n  - openapi/figma-files-api-openapi.yml\n  - openapi/figma-images-api-openapi.yml\n  - openapi/figma-me-api-openapi.yml\n  - openapi/figma-payments-api-openapi.yml\n  - openapi/figma-projects-api-openapi.yml\n  - openapi/figma-rest-api-openapi.yml\n  - openapi/figma-styles-api-openapi.yml\n  - openapi/figma-teams-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/authentication/figma-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
---
