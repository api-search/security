---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: jasper-da-com-attachments-api-openapi.yml
  format: yaml
  label: Jasper Attachments API
  slug: jasper-da-com-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-attachments-api-openapi.yml
- filename: jasper-da-com-audiences-api-openapi.yml
  format: yaml
  label: Jasper Audiences API
  slug: jasper-da-com-audiences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-audiences-api-openapi.yml
- filename: jasper-da-com-command-api-openapi.yml
  format: yaml
  label: Jasper Command API
  slug: jasper-da-com-command-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-command-api-openapi.yml
- filename: jasper-da-com-context-sources-api-openapi.yml
  format: yaml
  label: Jasper Context Sources API
  slug: jasper-da-com-context-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-context-sources-api-openapi.yml
- filename: jasper-da-com-documents-api-openapi.yml
  format: yaml
  label: Jasper Documents API
  slug: jasper-da-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-documents-api-openapi.yml
- filename: jasper-da-com-geo-api-openapi.yml
  format: yaml
  label: Jasper GEO API
  slug: jasper-da-com-geo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-geo-api-openapi.yml
- filename: jasper-da-com-image-templates-api-openapi.yml
  format: yaml
  label: Jasper Image Templates API
  slug: jasper-da-com-image-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-image-templates-api-openapi.yml
- filename: jasper-da-com-images-api-openapi.yml
  format: yaml
  label: Jasper Images API
  slug: jasper-da-com-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-images-api-openapi.yml
- filename: jasper-da-com-knowledge-api-openapi.yml
  format: yaml
  label: Jasper Knowledge API
  slug: jasper-da-com-knowledge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-knowledge-api-openapi.yml
- filename: jasper-da-com-products-api-openapi.yml
  format: yaml
  label: Jasper Products API
  slug: jasper-da-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-products-api-openapi.yml
- filename: jasper-da-com-projects-api-openapi.yml
  format: yaml
  label: Jasper Projects API
  slug: jasper-da-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-projects-api-openapi.yml
- filename: jasper-da-com-styles-api-openapi.yml
  format: yaml
  label: Jasper Styles API
  slug: jasper-da-com-styles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-styles-api-openapi.yml
- filename: jasper-da-com-tasks-api-openapi.yml
  format: yaml
  label: Jasper Tasks API
  slug: jasper-da-com-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-tasks-api-openapi.yml
- filename: jasper-da-com-templates-api-openapi.yml
  format: yaml
  label: Jasper Templates API
  slug: jasper-da-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-templates-api-openapi.yml
- filename: jasper-da-com-usage-api-openapi.yml
  format: yaml
  label: Jasper Usage API
  slug: jasper-da-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-usage-api-openapi.yml
- filename: jasper-da-com-users-api-openapi.yml
  format: yaml
  label: Jasper Users API
  slug: jasper-da-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-users-api-openapi.yml
- filename: jasper-da-com-voices-api-openapi.yml
  format: yaml
  label: Jasper Voices API
  slug: jasper-da-com-voices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-voices-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Jasper Da Com Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Jasper secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Jasper
provider_slug: jasper-da-com
scheme_count: 2
schemes:
- description: Workspace authentication using API key tokens in the X-API-Key header.
  in: header
  name: X-API-Key
  parameter: X-API-Key
  sources:
  - openapi/jasper-da-com-api-openapi.yml
  type: apiKey
- description: User-level authentication using OAuth bearer tokens in the Authorization header.
  flows:
  - authorizationUrl: https://api.jasper.ai/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.jasper.ai/oauth2/token
  name: oauth2
  sources:
  - openapi/jasper-da-com-api-openapi.yml
  type: oauth2
slug: jasper-da-com-authentication
source_filename: jasper-da-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: derived\nsource: openapi/jasper-da-com-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Workspace authentication using API key tokens in the X-API-Key header.\n  sources:\n  - openapi/jasper-da-com-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.jasper.ai/oauth2/authorize\n    tokenUrl: https://api.jasper.ai/oauth2/token\n    scopes: 2\n  description: User-level authentication using OAuth bearer tokens in the Authorization header.\n  sources:\n  - openapi/jasper-da-com-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/jasper-da-com/authentication/jasper-da-com-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- AI
- Marketing
- Automation
- Content
- Platform
- Company
---
