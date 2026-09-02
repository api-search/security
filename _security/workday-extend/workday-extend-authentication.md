---
api_key_in: []
api_specs:
- filename: workday-extend-app-configurations-api-openapi.yml
  format: yaml
  label: Workday Extend App Configurations API
  slug: workday-extend-app-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-app-configurations-api-openapi.yml
- filename: workday-extend-app-deployments-api-openapi.yml
  format: yaml
  label: Workday Extend App Deployments API
  slug: workday-extend-app-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-app-deployments-api-openapi.yml
- filename: workday-extend-app-versions-api-openapi.yml
  format: yaml
  label: Workday Extend App Versions API
  slug: workday-extend-app-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-app-versions-api-openapi.yml
- filename: workday-extend-apps-api-openapi.yml
  format: yaml
  label: Workday Extend Apps API
  slug: workday-extend-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-apps-api-openapi.yml
- filename: workday-extend-custom-object-definitions-api-openapi.yml
  format: yaml
  label: Workday Extend Custom Object Definitions API
  slug: workday-extend-custom-object-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-custom-object-definitions-api-openapi.yml
- filename: workday-extend-custom-object-fields-api-openapi.yml
  format: yaml
  label: Workday Extend Custom Object Fields API
  slug: workday-extend-custom-object-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-custom-object-fields-api-openapi.yml
- filename: workday-extend-custom-object-instances-api-openapi.yml
  format: yaml
  label: Workday Extend Custom Object Instances API
  slug: workday-extend-custom-object-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-custom-object-instances-api-openapi.yml
- filename: workday-extend-graph-query-api-openapi.yml
  format: yaml
  label: Workday Extend Graph Query API
  slug: workday-extend-graph-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-graph-query-api-openapi.yml
- filename: workday-extend-orchestration-executions-api-openapi.yml
  format: yaml
  label: Workday Extend Orchestration Executions API
  slug: workday-extend-orchestration-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-orchestration-executions-api-openapi.yml
- filename: workday-extend-orchestration-steps-api-openapi.yml
  format: yaml
  label: Workday Extend Orchestration Steps API
  slug: workday-extend-orchestration-steps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-orchestration-steps-api-openapi.yml
- filename: workday-extend-orchestration-triggers-api-openapi.yml
  format: yaml
  label: Workday Extend Orchestration Triggers API
  slug: workday-extend-orchestration-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-orchestration-triggers-api-openapi.yml
- filename: workday-extend-orchestrations-api-openapi.yml
  format: yaml
  label: Workday Extend Orchestrations API
  slug: workday-extend-orchestrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-orchestrations-api-openapi.yml
- filename: workday-extend-schema-introspection-api-openapi.yml
  format: yaml
  label: Workday Extend Schema Introspection API
  slug: workday-extend-schema-introspection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-schema-introspection-api-openapi.yml
- filename: workday-extend-wql-query-api-openapi.yml
  format: yaml
  label: Workday Extend WQL Query API
  slug: workday-extend-wql-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-wql-query-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Workday Extend Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Workday Extend secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Workday Extend
provider_slug: workday-extend
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://{baseUrl}/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://{baseUrl}/oauth2/{tenant}/token
  name: OAuth2
  sources:
  - openapi/workday-extend-custom-objects-openapi.yml
  - openapi/workday-extend-graph-api-openapi.yml
  - openapi/workday-extend-orchestration-openapi.yml
  - openapi/workday-extend-rest-api-openapi.yml
  type: oauth2
slug: workday-extend-authentication
source_filename: workday-extend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-extend-custom-objects-openapi.yml, openapi/workday-extend-graph-api-openapi.yml,\n  openapi/workday-extend-orchestration-openapi.yml, openapi/workday-extend-rest-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{baseUrl}/authorize\n    tokenUrl: https://{baseUrl}/oauth2/{tenant}/token\n    scopes: 2\n  sources:\n  - openapi/workday-extend-custom-objects-openapi.yml\n  - openapi/workday-extend-graph-api-openapi.yml\n  - openapi/workday-extend-orchestration-openapi.yml\n  - openapi/workday-extend-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/authentication/workday-extend-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Automation
- Custom Applications
- Enterprise
- Extensions
- HCM
- Integration
- Orchestration
- Platform-as-a-Service
---
