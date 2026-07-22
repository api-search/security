---
api_key_in:
- header
api_specs:
- filename: wherobots-cloud-openapi-original.json
  format: json
  label: Wherobots Cloud API
  slug: wherobots-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wherobots/refs/heads/main/openapi/wherobots-cloud-openapi-original.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Wherobots Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Wherobots secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Wherobots
provider_slug: wherobots
scheme_count: 3
schemes:
- description: Primary programmatic auth. A Wherobots-generated API key passed in the X-API-Key header (also read from the WHEROBOTS_API_KEY env var by the CLI and SDKs). Keys are created in Settings > API Keys, carry an expiration (default 1 year; presets 1h..4y), and can be created under a Service Principal for machine/service workloads. Any org member can create; admins can revoke org-wide.
  docs: https://docs.wherobots.com/get-started/wherobots-cloud/api-keys/
  in: header
  name: wherobotsApiKey
  parameter: X-API-Key
  sources:
  - openapi/wherobots-cloud-openapi-original.json
  type: apiKey
- description: Bearer access token accepted on the Wherobots Cloud API (used by the interactive API docs Authorize flow and OAuth-authenticated clients).
  name: bearerToken
  scheme: bearer
  sources:
  - openapi/wherobots-cloud-openapi-original.json
  type: http
- authorization_endpoint: https://login.cloud.wherobots.com/
  description: Browser OAuth sign-in (WorkOS AuthKit) used by the hosted MCP Server and the Wherobots Cloud console. On first connect the MCP client opens a browser to sign in to Wherobots and select an organization. Requires an existing account. Not declared in the OpenAPI securitySchemes (surfaced via the login.cloud.wherobots.com authorization endpoint).
  docs: https://docs.wherobots.com/develop/mcp/mcp-server-overview/
  flow: authorizationCode
  name: oauth2
  type: oauth2
slug: wherobots-authentication
source_filename: wherobots-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/wherobots-cloud-openapi-original.json\ndocs: https://docs.wherobots.com/get-started/wherobots-cloud/api-keys/\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: wherobotsApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: >-\n    Primary programmatic auth. A Wherobots-generated API key passed in the\n    X-API-Key header (also read from the WHEROBOTS_API_KEY env var by the CLI\n    and SDKs). Keys are created in Settings > API Keys, carry an expiration\n    (default 1 year; presets 1h..4y), and can be created under a Service\n    Principal for machine/service workloads. Any org member can create; admins\n    can revoke org-wide.\n  sources:\n  - openapi/wherobots-cloud-openapi-original.json\n  docs: https://docs.wherobots.com/get-started/wherobots-cloud/api-keys/\n- name: bearerToken\n  type: http\n  scheme:\
  \ bearer\n  description: >-\n    Bearer access token accepted on the Wherobots Cloud API (used by the\n    interactive API docs Authorize flow and OAuth-authenticated clients).\n  sources:\n  - openapi/wherobots-cloud-openapi-original.json\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  description: >-\n    Browser OAuth sign-in (WorkOS AuthKit) used by the hosted MCP Server and\n    the Wherobots Cloud console. On first connect the MCP client opens a browser\n    to sign in to Wherobots and select an organization. Requires an existing\n    account. Not declared in the OpenAPI securitySchemes (surfaced via the\n    login.cloud.wherobots.com authorization endpoint).\n  authorization_endpoint: https://login.cloud.wherobots.com/\n  docs: https://docs.wherobots.com/develop/mcp/mcp-server-overview/\nidentity:\n  service_principals: https://docs.wherobots.com/get-started/wherobots-cloud/service-principals/\n  sso: SAML-based SSO + passkeys (enterprise); https://docs.wherobots.com/get-started/organization-management/configuring-saml/\n\
  \  provider: WorkOS\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wherobots/refs/heads/main/authentication/wherobots-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Geospatial
- Spatial Analytics
- Apache Sedona
- Spatial SQL
- Geospatial AI
- Cloud Data Platform
- Raster
- GIS
---
