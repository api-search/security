---
anonymous_access: false
api_key_in: []
api_specs:
- filename: rendry-io-accounts-api-openapi.yml
  format: yaml
  label: rendry-io Accounts API
  slug: rendry-io-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-accounts-api-openapi.yml
- filename: rendry-io-assets-api-openapi.yml
  format: yaml
  label: rendry-io Assets API
  slug: rendry-io-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-assets-api-openapi.yml
- filename: rendry-io-batch-tasks-api-openapi.yml
  format: yaml
  label: rendry-io Batch Tasks API
  slug: rendry-io-batch-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-batch-tasks-api-openapi.yml
- filename: rendry-io-capabilities-api-openapi.yml
  format: yaml
  label: rendry-io Capabilities API
  slug: rendry-io-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-capabilities-api-openapi.yml
- filename: rendry-io-components-api-openapi.yml
  format: yaml
  label: rendry-io Components API
  slug: rendry-io-components-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-components-api-openapi.yml
- filename: rendry-io-design-guide-api-openapi.yml
  format: yaml
  label: rendry-io Design Guide API
  slug: rendry-io-design-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-design-guide-api-openapi.yml
- filename: rendry-io-documents-api-openapi.yml
  format: yaml
  label: rendry-io Documents API
  slug: rendry-io-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-documents-api-openapi.yml
- filename: rendry-io-embed-api-openapi.yml
  format: yaml
  label: rendry-io Embed API
  slug: rendry-io-embed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-embed-api-openapi.yml
- filename: rendry-io-files-api-openapi.yml
  format: yaml
  label: rendry-io Files API
  slug: rendry-io-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-files-api-openapi.yml
- filename: rendry-io-generations-api-openapi.yml
  format: yaml
  label: rendry-io Generations API
  slug: rendry-io-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-generations-api-openapi.yml
- filename: rendry-io-images-api-openapi.yml
  format: yaml
  label: rendry-io Images API
  slug: rendry-io-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-images-api-openapi.yml
- filename: rendry-io-mcp-api-openapi.yml
  format: yaml
  label: rendry-io MCP API
  slug: rendry-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-mcp-api-openapi.yml
- filename: rendry-io-presets-api-openapi.yml
  format: yaml
  label: rendry-io Presets API
  slug: rendry-io-presets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-presets-api-openapi.yml
- filename: rendry-io-principal-api-openapi.yml
  format: yaml
  label: rendry-io Principal API
  slug: rendry-io-principal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-principal-api-openapi.yml
- filename: rendry-io-render-api-openapi.yml
  format: yaml
  label: rendry-io Render API
  slug: rendry-io-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-render-api-openapi.yml
- filename: rendry-io-rendering-api-openapi.yml
  format: yaml
  label: rendry-io Rendering API
  slug: rendry-io-rendering-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-rendering-api-openapi.yml
- filename: rendry-io-templates-api-openapi.yml
  format: yaml
  label: rendry-io Templates API
  slug: rendry-io-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-templates-api-openapi.yml
- filename: rendry-io-u-api-openapi.yml
  format: yaml
  label: rendry-io U API
  slug: rendry-io-u-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-u-api-openapi.yml
- filename: rendry-io-user-api-openapi.yml
  format: yaml
  label: rendry-io User API
  slug: rendry-io-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-user-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Rendry Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: rendry-io declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: rendry-io
provider_slug: rendry-io
scheme_count: 2
schemes:
- description: Bearer token API key (sk_live_...)
  in: header
  name: Authorization
  type: apiKey
- description: OAuth 2.1 for MCP clients
  flows:
    authorizationCode:
      authorizationUrl: https://rendry.io/oauth/authorize
      scopes: {}
      tokenUrl: https://rendry.io/oauth/token
  type: oauth2
slug: rendry-io-authentication
source_filename: rendry-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://rendry.io/docs/authentication\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: Bearer token API key (sk_live_...)\n  - type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://rendry.io/oauth/authorize\n        tokenUrl: https://rendry.io/oauth/token\n        scopes: {}\n    description: OAuth 2.1 for MCP clients\n"
source_yaml_url: https://artifacts.apis.io/rendry-io/authentication/rendry-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Image Rendering
- PDF Generation
- Template Engine
- API
- AI Integration
---
