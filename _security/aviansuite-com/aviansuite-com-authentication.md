---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aviansuite-com-admin-api-openapi.yml
  format: yaml
  label: AvianSuite Admin API
  slug: aviansuite-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aviansuite-com/openapi/aviansuite-com-admin-api-openapi.yml
- filename: aviansuite-com-events-api-openapi.yml
  format: yaml
  label: AvianSuite Events API
  slug: aviansuite-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aviansuite-com/openapi/aviansuite-com-events-api-openapi.yml
- filename: aviansuite-com-health-api-openapi.yml
  format: yaml
  label: AvianSuite Health API
  slug: aviansuite-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aviansuite-com/openapi/aviansuite-com-health-api-openapi.yml
- filename: aviansuite-com-refs-api-openapi.yml
  format: yaml
  label: AvianSuite Refs API
  slug: aviansuite-com-refs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aviansuite-com/openapi/aviansuite-com-refs-api-openapi.yml
- filename: aviansuite-com-root-api-openapi.yml
  format: yaml
  label: AvianSuite Root API
  slug: aviansuite-com-root-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aviansuite-com/openapi/aviansuite-com-root-api-openapi.yml
auth_types: []
description: AvianSuite authentication uses OAuth2 service_auth flow for agents.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: AvianSuite Authentication
name_suffix: Authentication
oauth_flows: []
overview: AvianSuite declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AvianSuite
provider_slug: aviansuite-com
scheme_count: 1
schemes:
- authorizationUrl: https://app.aviansuite.com/agent/identity
  flow: authorization_code
  scopes: {}
  tokenUrl: https://app.aviansuite.com/oauth/token
  type: oauth2
slug: aviansuite-com-authentication
source_filename: aviansuite-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://aviansuite.com/auth.md\ndescription: \"AvianSuite authentication uses OAuth2 service_auth flow for agents.\"\n\ndocs: https://aviansuite.com/auth.md\nschemes:\n  - type: oauth2\n    flow: authorization_code\n    authorizationUrl: https://app.aviansuite.com/agent/identity\n    tokenUrl: https://app.aviansuite.com/oauth/token\n    scopes: {}\n"
source_yaml_url: https://artifacts.apis.io/aviansuite-com/authentication/aviansuite-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Agents
- Business Data
- Automation
- Platform
---
