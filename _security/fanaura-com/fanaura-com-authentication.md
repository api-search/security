---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: fanaura-com-careers-api-openapi.yml
  format: yaml
  label: Fanaura Careers API
  slug: fanaura-com-careers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanaura-com/openapi/fanaura-com-careers-api-openapi.yml
- filename: fanaura-com-demo-api-openapi.yml
  format: yaml
  label: Fanaura Demo API
  slug: fanaura-com-demo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanaura-com/openapi/fanaura-com-demo-api-openapi.yml
- filename: fanaura-com-legal-api-openapi.yml
  format: yaml
  label: Fanaura Legal API
  slug: fanaura-com-legal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanaura-com/openapi/fanaura-com-legal-api-openapi.yml
- filename: fanaura-com-llms-full-txt-api-openapi.yml
  format: yaml
  label: Fanaura Llms Full.txt API
  slug: fanaura-com-llms-full-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanaura-com/openapi/fanaura-com-llms-full-txt-api-openapi.yml
- filename: fanaura-com-llms-txt-api-openapi.yml
  format: yaml
  label: Fanaura Llms.txt API
  slug: fanaura-com-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanaura-com/openapi/fanaura-com-llms-txt-api-openapi.yml
- filename: fanaura-com-mcp-api-openapi.yml
  format: yaml
  label: Fanaura MCP API
  slug: fanaura-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanaura-com/openapi/fanaura-com-mcp-api-openapi.yml
- filename: fanaura-com-openapi-json-api-openapi.yml
  format: yaml
  label: Fanaura Openapi.json API
  slug: fanaura-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanaura-com/openapi/fanaura-com-openapi-json-api-openapi.yml
- filename: fanaura-com-privacy-policy-txt-api-openapi.yml
  format: yaml
  label: Fanaura Privacy Policy.txt API
  slug: fanaura-com-privacy-policy-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanaura-com/openapi/fanaura-com-privacy-policy-txt-api-openapi.yml
- filename: fanaura-com-revalidate-api-openapi.yml
  format: yaml
  label: Fanaura Revalidate API
  slug: fanaura-com-revalidate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanaura-com/openapi/fanaura-com-revalidate-api-openapi.yml
- filename: fanaura-com-sitemap-xml-api-openapi.yml
  format: yaml
  label: Fanaura Sitemap.xml API
  slug: fanaura-com-sitemap-xml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanaura-com/openapi/fanaura-com-sitemap-xml-api-openapi.yml
- filename: fanaura-com-well-known-api-openapi.yml
  format: yaml
  label: Fanaura .well Known API
  slug: fanaura-com-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fanaura-com/openapi/fanaura-com-well-known-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Fanaura Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Fanaura secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Fanaura
provider_slug: fanaura-com
scheme_count: 2
schemes:
- description: OAuth 2.0 for https://app.fanaura.com/mcp. Authorization code with PKCE (S256). Request only the scope the task needs. Do not request every scope in this list.
  flows:
  - authorizationUrl: https://app.fanaura.com/oauth/mcp/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://app.fanaura.com/api/oauth/mcp/token
  name: fanauraMcpOAuth
  sources:
  - openapi/fanaura-com-openapi.json
  type: oauth2
- description: Shared secret for the website cache hook. Not an OAuth scope.
  in: header
  name: revalidateSecret
  parameter: x-revalidate-secret
  sources:
  - openapi/fanaura-com-openapi.json
  type: apiKey
slug: fanaura-com-authentication
source_filename: fanaura-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/fanaura-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: fanauraMcpOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.fanaura.com/oauth/mcp/authorize\n    tokenUrl: https://app.fanaura.com/api/oauth/mcp/token\n    scopes: 3\n  description: OAuth 2.0 for https://app.fanaura.com/mcp. Authorization code with PKCE (S256).\n    Request only the scope the task needs. Do not request every scope in this list.\n  sources:\n  - openapi/fanaura-com-openapi.json\n- name: revalidateSecret\n  type: apiKey\n  in: header\n  parameter: x-revalidate-secret\n  description: Shared secret for the website cache hook. Not an OAuth scope.\n  sources:\n  - openapi/fanaura-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/fanaura-com/authentication/fanaura-com-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Instagram DM automation
- Music marketing
- Release marketing
- Business marketing
---
