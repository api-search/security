---
anonymous_access: false
api_key_in: []
api_specs:
- filename: appmixer-accounts-api-openapi.yml
  format: yaml
  label: Appmixer Accounts API
  slug: appmixer-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-accounts-api-openapi.yml
- filename: appmixer-apps-api-openapi.yml
  format: yaml
  label: Appmixer Apps API
  slug: appmixer-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-apps-api-openapi.yml
- filename: appmixer-authentication-api-openapi.yml
  format: yaml
  label: Appmixer Authentication API
  slug: appmixer-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-authentication-api-openapi.yml
- filename: appmixer-files-api-openapi.yml
  format: yaml
  label: Appmixer Files API
  slug: appmixer-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-files-api-openapi.yml
- filename: appmixer-flows-api-openapi.yml
  format: yaml
  label: Appmixer Flows API
  slug: appmixer-flows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-flows-api-openapi.yml
- filename: appmixer-insights-api-openapi.yml
  format: yaml
  label: Appmixer Insights API
  slug: appmixer-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-insights-api-openapi.yml
- filename: appmixer-acl-api-openapi.yml
  format: yaml
  label: Appmixer ACL API
  slug: appmixer-acl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-acl-api-openapi.yml
- filename: appmixer-audit-logs-api-openapi.yml
  format: yaml
  label: Appmixer Audit Logs API
  slug: appmixer-audit-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-audit-logs-api-openapi.yml
- filename: appmixer-automation-hub-api-openapi.yml
  format: yaml
  label: Appmixer Automation Hub API
  slug: appmixer-automation-hub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-automation-hub-api-openapi.yml
- filename: appmixer-config-api-openapi.yml
  format: yaml
  label: Appmixer Config API
  slug: appmixer-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-config-api-openapi.yml
- filename: appmixer-connector-configuration-api-openapi.yml
  format: yaml
  label: Appmixer Connector Configuration API
  slug: appmixer-connector-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-connector-configuration-api-openapi.yml
- filename: appmixer-integration-categories-api-openapi.yml
  format: yaml
  label: Appmixer Integration Categories API
  slug: appmixer-integration-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-integration-categories-api-openapi.yml
- filename: appmixer-modifiers-api-openapi.yml
  format: yaml
  label: Appmixer Modifiers API
  slug: appmixer-modifiers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-modifiers-api-openapi.yml
- filename: appmixer-public-files-api-openapi.yml
  format: yaml
  label: Appmixer Public Files API
  slug: appmixer-public-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-public-files-api-openapi.yml
- filename: appmixer-unprocessed-messages-api-openapi.yml
  format: yaml
  label: Appmixer Unprocessed Messages API
  slug: appmixer-unprocessed-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-unprocessed-messages-api-openapi.yml
- filename: appmixer-user-api-openapi.yml
  format: yaml
  label: Appmixer User API
  slug: appmixer-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-user-api-openapi.yml
- filename: appmixer-user-groups-api-openapi.yml
  format: yaml
  label: Appmixer User Groups API
  slug: appmixer-user-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-user-groups-api-openapi.yml
- filename: appmixer-variables-api-openapi.yml
  format: yaml
  label: Appmixer Variables API
  slug: appmixer-variables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-variables-api-openapi.yml
- filename: appmixer-datastores-api-openapi.yml
  format: yaml
  label: Appmixer Datastores API
  slug: appmixer-datastores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-datastores-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Appmixer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Appmixer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Appmixer
provider_slug: appmixer
scheme_count: 1
schemes:
- description: 'Access token obtained from the /user/auth endpoint. Pass as Authorization: Bearer {token} header.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/appmixer-api-openapi.yml
  type: http
slug: appmixer-authentication
source_filename: appmixer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/appmixer-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Access token obtained from the /user/auth endpoint. Pass as Authorization: Bearer\n    {token} header.'\n  sources:\n  - openapi/appmixer-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/appmixer/authentication/appmixer-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Agents
- Automation
- Embedded iPaaS
- Integration
- Low-Code
- Workflows
---
