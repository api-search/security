---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aislesinventory-com-agent-api-openapi.yml
  format: yaml
  label: Aisles Inc. Agent API
  slug: aislesinventory-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aislesinventory-com/openapi/aislesinventory-com-agent-api-openapi.yml
- filename: aislesinventory-com-jobs-api-openapi.yml
  format: yaml
  label: Aisles Inc. Jobs API
  slug: aislesinventory-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aislesinventory-com/openapi/aislesinventory-com-jobs-api-openapi.yml
- filename: aislesinventory-com-sandbox-api-openapi.yml
  format: yaml
  label: Aisles Inc. Sandbox API
  slug: aislesinventory-com-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aislesinventory-com/openapi/aislesinventory-com-sandbox-api-openapi.yml
- filename: aislesinventory-com-search-api-openapi.yml
  format: yaml
  label: Aisles Inc. Search API
  slug: aislesinventory-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aislesinventory-com/openapi/aislesinventory-com-search-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Aisles Inc. Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Aisles Inc. secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Aisles Inc.
provider_slug: aislesinventory-com
scheme_count: 1
schemes:
- description: 'Optional agent sign-in (https://aislesinventory.com/auth.md): register at /oauth/register, then client credentials.'
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://aislesinventory.com/oauth/token
  name: oauth2
  sources:
  - openapi/aislesinventory-com-openapi.json
  - openapi/aislesinventory-com-sandbox-openapi.json
  type: oauth2
slug: aislesinventory-com-authentication
source_filename: aislesinventory-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/aislesinventory-com-openapi.json, openapi/aislesinventory-com-sandbox-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://aislesinventory.com/oauth/token\n    scopes: 2\n  description: 'Optional agent sign-in (https://aislesinventory.com/auth.md): register at /oauth/register,\n    then client credentials.'\n  sources:\n  - openapi/aislesinventory-com-openapi.json\n  - openapi/aislesinventory-com-sandbox-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/aislesinventory-com/authentication/aislesinventory-com-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Inventory
- Retail
- Stocks
- US
---
