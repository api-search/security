---
anonymous_access: false
api_key_in: []
api_specs:
- filename: alma-food-discovery-api-openapi.yml
  format: yaml
  label: Alma Discovery API
  slug: alma-food-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alma-food/openapi/alma-food-discovery-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Alma Food Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Alma secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Alma
provider_slug: alma-food
scheme_count: 1
schemes:
- description: OAuth for the Alma MCP server at https://mcp.alma.food. Request only the scopes needed for the job.
  flows:
  - authorizationUrl: https://mcp.alma.food/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://mcp.alma.food/token
  name: almaMcpOAuth
  sources:
  - openapi/alma-food-openapi.json
  type: oauth2
slug: alma-food-authentication
source_filename: alma-food-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/alma-food-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: almaMcpOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.alma.food/authorize\n    tokenUrl: https://mcp.alma.food/token\n    scopes: 2\n  description: OAuth for the Alma MCP server at https://mcp.alma.food. Request only the scopes\n    needed for the job.\n  sources:\n  - openapi/alma-food-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/alma-food/authentication/alma-food-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Nutrition
- Artificial Intelligence
- Health
- Food Tracking
- Personalization
- Company
---
