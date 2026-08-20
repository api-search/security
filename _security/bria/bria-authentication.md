---
api_key_in:
- header
api_specs:
- filename: bria-automotive-endpoints-api-openapi.yml
  format: yaml
  label: Bria Automotive Endpoints API
  slug: bria-automotive-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-automotive-endpoints-api-openapi.yml
- filename: bria-dataset-api-openapi.yml
  format: yaml
  label: Bria Dataset API
  slug: bria-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-dataset-api-openapi.yml
- filename: bria-editing-endpoints-api-openapi.yml
  format: yaml
  label: Bria Editing Endpoints API
  slug: bria-editing-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-editing-endpoints-api-openapi.yml
- filename: bria-endpoints-api-openapi.yml
  format: yaml
  label: Bria Endpoints API
  slug: bria-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-endpoints-api-openapi.yml
- filename: bria-image-attribution-api-openapi.yml
  format: yaml
  label: Bria Image Attribution API
  slug: bria-image-attribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-image-attribution-api-openapi.yml
- filename: bria-image-generation-api-openapi.yml
  format: yaml
  label: Bria Image Generation API
  slug: bria-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-image-generation-api-openapi.yml
- filename: bria-masking-endpoints-api-openapi.yml
  format: yaml
  label: Bria Masking Endpoints API
  slug: bria-masking-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-masking-endpoints-api-openapi.yml
- filename: bria-model-api-openapi.yml
  format: yaml
  label: Bria Model API
  slug: bria-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-model-api-openapi.yml
- filename: bria-product-endpoints-api-openapi.yml
  format: yaml
  label: Bria Product Endpoints API
  slug: bria-product-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-product-endpoints-api-openapi.yml
- filename: bria-project-api-openapi.yml
  format: yaml
  label: Bria Project API
  slug: bria-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-project-api-openapi.yml
- filename: bria-v2-endpoints-api-openapi.yml
  format: yaml
  label: Bria v2 endpoints API
  slug: bria-v2-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-v2-endpoints-api-openapi.yml
- filename: bria-video-attribution-api-openapi.yml
  format: yaml
  label: Bria Video Attribution API
  slug: bria-video-attribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-video-attribution-api-openapi.yml
- filename: bria-video-generation-api-openapi.yml
  format: yaml
  label: Bria Video Generation API
  slug: bria-video-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/openapi/bria-video-generation-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Bria Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refresh_token
- device_code
overview: Bria secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refresh_token, and device_code flow(s).
provider_name: Bria
provider_slug: bria
scheme_count: 3
schemes:
- declared_as: header parameter
  in: header
  name: api_token
  note: Issued and rotated from the Bria console; separate keys can be minted for production, staging, MCP and ComfyUI use. Tokens are long-lived and Bria states no rotation logic is required.
  operations: 97
  parameter: api_token
  required: true
  sources:
  - openapi/bria-image-generation-openapi-original.yml
  - openapi/bria-image-editing-openapi-original.yml
  - openapi/bria-video-editing-openapi-original.yml
  - openapi/bria-product-shot-editing-openapi-original.yml
  - openapi/bria-tailored-generation-openapi-original.yml
  - openapi/bria-ad-generation-openapi-original.yml
  - openapi/bria-image-onboarding-openapi-original.yml
  - openapi/bria-status-openapi-original.yml
  - openapi/bria-ai-search-deperecated-openapi-original.yml
  type: apiKey
- name: BearerAuth
  note: The Attribution Service is the only spec that declares a real securityScheme.
  scheme: bearer
  sources:
  - openapi/bria-attribution-service-openapi-original.yml
  type: http
- discovery: https://engine.prod.bria-api.com/.well-known/oauth-authorization-server
  dynamic_client_registration: https://engine.prod.bria-api.com/v2/auth/register
  flows:
  - authorizationUrl: https://engine.prod.bria-api.com/v2/auth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://engine.prod.bria-api.com/v2/auth/token
  - deviceAuthorizationUrl: https://engine.prod.bria-api.com/v2/auth/device/authorize
    flow: deviceCode
  metadata_spec: RFC 8414
  name: OAuth2
  note: Discovered by probe, not declared in any OpenAPI. Used for the OAuth-based bearer token that the MCP server accepts in its authorization_token parameter.
  registration_spec: RFC 7591
  sources:
  - well-known/bria-engine-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_post
  - none
  type: oauth2
slug: bria-authentication
source_filename: bria-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: searched\nsource: openapi/*-openapi-original.yml + https://docs.bria.ai/mcp-authentication\ndocs: https://docs.bria.ai/mcp-authentication\nconsole: https://platform.bria.ai/organization-management/api-keys\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - refresh_token\n  - device_code\n  primary: >-\n    A static, long-lived API token sent in the api_token request header. It is a required header\n    parameter on 97 of 104 published operations but is declared as a plain header parameter, not as\n    an OpenAPI securityScheme, so a generator reading only components.securitySchemes will not\n    emit auth for those operations.\nschemes:\n- name: api_token\n  type: apiKey\n  in: header\n  parameter: api_token\n  required: true\n  declared_as: header parameter\n  operations: 97\n  sources:\n  - openapi/bria-image-generation-openapi-original.yml\n  - openapi/bria-image-editing-openapi-original.yml\n\
  \  - openapi/bria-video-editing-openapi-original.yml\n  - openapi/bria-product-shot-editing-openapi-original.yml\n  - openapi/bria-tailored-generation-openapi-original.yml\n  - openapi/bria-ad-generation-openapi-original.yml\n  - openapi/bria-image-onboarding-openapi-original.yml\n  - openapi/bria-status-openapi-original.yml\n  - openapi/bria-ai-search-deperecated-openapi-original.yml\n  note: >-\n    Issued and rotated from the Bria console; separate keys can be minted for production, staging,\n    MCP and ComfyUI use. Tokens are long-lived and Bria states no rotation logic is required.\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/bria-attribution-service-openapi-original.yml\n  note: The Attribution Service is the only spec that declares a real securityScheme.\n- name: OAuth2\n  type: oauth2\n  discovery: https://engine.prod.bria-api.com/.well-known/oauth-authorization-server\n  metadata_spec: RFC 8414\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://engine.prod.bria-api.com/v2/auth/authorize\n    tokenUrl: https://engine.prod.bria-api.com/v2/auth/token\n    pkce: S256\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://engine.prod.bria-api.com/v2/auth/device/authorize\n  dynamic_client_registration: https://engine.prod.bria-api.com/v2/auth/register\n  registration_spec: RFC 7591\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - none\n  sources:\n  - well-known/bria-engine-oauth-authorization-server.json\n  note: >-\n    Discovered by probe, not declared in any OpenAPI. Used for the OAuth-based bearer token that\n    the MCP server accepts in its authorization_token parameter.\nmcp:\n  url: https://mcp.prod.bria-api.com/mcp\n  methods:\n  - api_token header (static API key)\n  - OAuth 2.0 bearer token (authorization_token)\n  anonymous_tools_list: 401\n  anonymous_response: 'either API key or Bearer token is required'\n  authorization_server: https://mcp.prod.bria-api.com/.well-known/oauth-authorization-server\n\
  gaps:\n- >-\n  api_token is not modelled as an OpenAPI securityScheme in nine of the ten specs, so\n  securitySchemes-defined and securitySchemes-applied contract checks fail even though every\n  operation is in fact authenticated.\n- >-\n  No /.well-known/oauth-protected-resource (RFC 9728) on the MCP host, so an MCP client cannot\n  discover the authorization server from the resource.\nx-evidence:\n  fetched: '2026-08-08'\n  probes:\n  - url: https://engine.prod.bria-api.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://mcp.prod.bria-api.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://mcp.prod.bria-api.com/mcp\n    http_status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bria/refs/heads/main/authentication/bria-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Artificial Intelligence
- Generative AI
- Image
- Image-Generation
- Image Editing
- Video
- Machine-Learning
- Media
- Content
- Agents
- MCP
---
