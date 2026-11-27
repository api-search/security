---
anonymous_access: false
api_key_in: []
api_specs:
- filename: backworkhealth-com-agent-tools-api-openapi.yml
  format: yaml
  label: Backwork Agent Tools API
  slug: backworkhealth-com-agent-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backworkhealth-com/openapi/backworkhealth-com-agent-tools-api-openapi.yml
- filename: backworkhealth-com-certified-releases-api-openapi.yml
  format: yaml
  label: Backwork Certified Releases API
  slug: backworkhealth-com-certified-releases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backworkhealth-com/openapi/backworkhealth-com-certified-releases-api-openapi.yml
- filename: backworkhealth-com-claims-api-openapi.yml
  format: yaml
  label: Backwork Claims API
  slug: backworkhealth-com-claims-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backworkhealth-com/openapi/backworkhealth-com-claims-api-openapi.yml
- filename: backworkhealth-com-codes-api-openapi.yml
  format: yaml
  label: Backwork Codes API
  slug: backworkhealth-com-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backworkhealth-com/openapi/backworkhealth-com-codes-api-openapi.yml
- filename: backworkhealth-com-compliance-api-openapi.yml
  format: yaml
  label: Backwork Compliance API
  slug: backworkhealth-com-compliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backworkhealth-com/openapi/backworkhealth-com-compliance-api-openapi.yml
- filename: backworkhealth-com-coverage-api-openapi.yml
  format: yaml
  label: Backwork Coverage API
  slug: backworkhealth-com-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backworkhealth-com/openapi/backworkhealth-com-coverage-api-openapi.yml
- filename: backworkhealth-com-drugs-api-openapi.yml
  format: yaml
  label: Backwork Drugs API
  slug: backworkhealth-com-drugs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backworkhealth-com/openapi/backworkhealth-com-drugs-api-openapi.yml
- filename: backworkhealth-com-health-api-openapi.yml
  format: yaml
  label: Backwork Health API
  slug: backworkhealth-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backworkhealth-com/openapi/backworkhealth-com-health-api-openapi.yml
- filename: backworkhealth-com-policies-api-openapi.yml
  format: yaml
  label: Backwork Policies API
  slug: backworkhealth-com-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backworkhealth-com/openapi/backworkhealth-com-policies-api-openapi.yml
- filename: backworkhealth-com-prior-auth-api-openapi.yml
  format: yaml
  label: Backwork Prior Auth API
  slug: backworkhealth-com-prior-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backworkhealth-com/openapi/backworkhealth-com-prior-auth-api-openapi.yml
- filename: backworkhealth-com-reference-api-openapi.yml
  format: yaml
  label: Backwork Reference API
  slug: backworkhealth-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backworkhealth-com/openapi/backworkhealth-com-reference-api-openapi.yml
- filename: backworkhealth-com-spending-api-openapi.yml
  format: yaml
  label: Backwork Spending API
  slug: backworkhealth-com-spending-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backworkhealth-com/openapi/backworkhealth-com-spending-api-openapi.yml
- filename: backworkhealth-com-webhooks-api-openapi.yml
  format: yaml
  label: Backwork Webhooks API
  slug: backworkhealth-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backworkhealth-com/openapi/backworkhealth-com-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Backwork Authentication
name_suffix: Authentication
oauth_flows: []
overview: Backwork declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Backwork
provider_slug: backworkhealth-com
scheme_count: 2
schemes:
- description: Bearer API key for live and test keys.
  in: header
  name: Authorization
  type: apiKey
- description: OAuth for MCP clients.
  flows:
    authorizationCode:
      authorizationUrl: https://backworkhealth.com/mcp/authorize
      scopes:
        backwork:mcp: Read/write access via MCP.
      tokenUrl: https://backworkhealth.com/mcp/token
  type: oauth2
slug: backworkhealth-com-authentication
source_filename: backworkhealth-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://developers.backworkhealth.com/docs/authentication\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: Bearer API key for live and test keys.\n  - type: oauth2\n    description: OAuth for MCP clients.\n    flows:\n      authorizationCode:\n        authorizationUrl: https://backworkhealth.com/mcp/authorize\n        tokenUrl: https://backworkhealth.com/mcp/token\n        scopes:\n          backwork:mcp: Read/write access via MCP.\n"
source_yaml_url: https://artifacts.apis.io/backworkhealth-com/authentication/backworkhealth-com-authentication.yml
summary_line: 2 schemes
tags:
- Healthcare
- Insurance
- Policy
- Medicare
- Compliance
---
