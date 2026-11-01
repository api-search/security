---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gtm-agent-api-v1-api-openapi.yml
  format: yaml
  label: Agent API
  slug: agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gtm/openapi/gtm-agent-api-v1-api-openapi.yml
- filename: gtm-copilot-api-v1-api-openapi.yml
  format: yaml
  label: Copilot API
  slug: copilot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gtm/openapi/gtm-copilot-api-v1-api-openapi.yml
- filename: gtm-data-api-v1-api-openapi.yml
  format: yaml
  label: Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gtm/openapi/gtm-data-api-v1-api-openapi.yml
- filename: gtm-data-quality-api-v1-api-openapi.yml
  format: yaml
  label: Data Quality API
  slug: data-quality-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gtm/openapi/gtm-data-quality-api-v1-api-openapi.yml
- filename: gtm-studio-api-v1-api-openapi.yml
  format: yaml
  label: Studio API
  slug: studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gtm/openapi/gtm-studio-api-v1-api-openapi.yml
- filename: gtm-marketing-api-v1-api-openapi.yml
  format: yaml
  label: Marketing API
  slug: marketing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gtm/openapi/gtm-marketing-api-v1-api-openapi.yml
- filename: gtm-platform-api-v1-api-openapi.yml
  format: yaml
  label: Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gtm/openapi/gtm-platform-api-v1-api-openapi.yml
- filename: gtm-vertical-datasets-api-v1-api-openapi.yml
  format: yaml
  label: Vertical Datasets API
  slug: vertical-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gtm/openapi/gtm-vertical-datasets-api-v1-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Gtm Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ZoomInfo secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ZoomInfo
provider_slug: gtm
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://login.zoominfo.com
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://okta-login.zoominfo.com/oauth2/default/v1/token
  name: OAuth2Auth
  sources:
  - openapi/gtm-agent-api-v1-api-openapi.yml
  - openapi/gtm-copilot-api-v1-api-openapi.yml
  - openapi/gtm-data-api-v1-api-openapi.yml
  - openapi/gtm-data-quality-api-v1-api-openapi.yml
  - openapi/gtm-marketing-api-v1-api-openapi.yml
  - openapi/gtm-platform-api-v1-api-openapi.yml
  - openapi/gtm-studio-api-v1-api-openapi.yml
  - openapi/gtm-vertical-datasets-api-v1-api-openapi.yml
  type: oauth2
slug: gtm-authentication
source_filename: gtm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: derived\nsource: openapi/gtm-agent-api-v1-api-openapi.yml, openapi/gtm-copilot-api-v1-api-openapi.yml,\n  openapi/gtm-data-api-v1-api-openapi.yml, openapi/gtm-data-quality-api-v1-api-openapi.yml,\n  openapi/gtm-marketing-api-v1-api-openapi.yml, openapi/gtm-platform-api-v1-api-openapi.yml,\n  openapi/gtm-studio-api-v1-api-openapi.yml, openapi/gtm-vertical-datasets-api-v1-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2Auth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.zoominfo.com\n    tokenUrl: https://okta-login.zoominfo.com/oauth2/default/v1/token\n    scopes: 3\n  sources:\n  - openapi/gtm-agent-api-v1-api-openapi.yml\n  - openapi/gtm-copilot-api-v1-api-openapi.yml\n  - openapi/gtm-data-api-v1-api-openapi.yml\n  - openapi/gtm-data-quality-api-v1-api-openapi.yml\n  - openapi/gtm-marketing-api-v1-api-openapi.yml\n  - openapi/gtm-platform-api-v1-api-openapi.yml\n\
  \  - openapi/gtm-studio-api-v1-api-openapi.yml\n  - openapi/gtm-vertical-datasets-api-v1-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/gtm/authentication/gtm-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- B2B
- Data
- Sales
---
