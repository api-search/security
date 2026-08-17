---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Kentico Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kentico secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kentico
provider_slug: kentico
scheme_count: 4
schemes:
- docs: https://docs.kentico.com/documentation/developers-and-admins/configuration/headless-channel-management
  format: Bearer <ApiKey>
  guidance: Kentico explicitly recommends NOT placing the key in a browser client — proxy GraphQL requests through a backend that adds the Authorization header, because a key sent from a public page is visible to anyone.
  in: header
  managed_in: Xperience administration → Channel management → the headless channel → API keys tab. Requires the "Manage headless channel API keys" permission.
  name: HeadlessChannelApiKey
  parameter_name: Authorization
  revocation: Keys can be disabled or deleted; disabling revokes access immediately and further requests with that key return an authorization error.
  scope: per headless channel
  surface: Headless channel GraphQL API
  type: apiKey
- docs: https://docs.kentico.com/documentation/developers-and-admins/deployment/deploy-to-the-saas-environment
  format: Bearer <PERSONAL_ACCESS_TOKEN>
  host: https://xperience-portal.com
  name: XperiencePortalPAT
  parameter_name: Authorization
  roles: Uploads to non-production environments and (in extraordinary circumstances) production require the DevOps Engineer or Tenant Administrator role.
  scheme: bearer
  scope: per Xperience Portal user; project addressed by PROJECT_GUID in the path
  surface: Xperience Portal API (SaaS deployment)
  type: http
- configured_by: ManagementApiOptions.Secret passed to AddKenticoManagementApi() in Program.cs; supplied to the MCP server as the MANAGEMENT_API_SECRET environment variable.
  docs: https://docs.kentico.com/documentation/developers-and-admins/api/management-api/configure-management-mcp-server
  format: shared secret, minimum 32 characters
  in: header
  name: ManagementApiSecret
  status: preview
  surface: Management API (preview) + Management MCP server
  type: apiKey
  warning: Kentico states the management API provides only basic authentication and NO per-operation authorization, and must not be enabled on production or any publicly reachable instance. It is a local-development surface.
- docs: https://docs.kentico.com/k12sp/integrating-3rd-party-systems/kentico-rest-service/authenticating-rest-requests
  format: Base64-encoded username:password, or a hash parameter for public endpoints
  name: RestServiceBasic
  scheme: basic
  surface: Kentico REST service (Kentico 12/13 line)
  type: http
slug: kentico-authentication
source_filename: kentico-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/ (none present) — profile assembled from Kentico's own documentation\ndocs:\n  - https://docs.kentico.com/documentation/developers-and-admins/configuration/headless-channel-management\n  - https://docs.kentico.com/documentation/developers-and-admins/api/management-api/configure-management-mcp-server\n  - https://docs.kentico.com/documentation/developers-and-admins/deployment/deploy-to-the-saas-environment\n  - https://docs.kentico.com/k12sp/integrating-3rd-party-systems/kentico-rest-service/authenticating-rest-requests\nnote: >-\n  Kentico publishes no OpenAPI, so derive-authentication.py found zero security\n  schemes (it aggregates OpenAPI securitySchemes and this repo has none). This\n  profile is SEARCHED from the documentation instead. Xperience by Kentico is\n  customer-deployed software: three of the four schemes below are enforced by\n  the customer's own instance, and only the Xperience Portal API is\n  authenticated\
  \ against a host Kentico operates.\n\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  http_schemes: [bearer, basic]\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n\nschemes:\n  - name: HeadlessChannelApiKey\n    type: apiKey\n    in: header\n    parameter_name: Authorization\n    format: \"Bearer <ApiKey>\"\n    surface: Headless channel GraphQL API\n    scope: per headless channel\n    managed_in: >-\n      Xperience administration → Channel management → the headless channel →\n      API keys tab. Requires the \"Manage headless channel API keys\" permission.\n    revocation: >-\n      Keys can be disabled or deleted; disabling revokes access immediately and\n      further requests with that key return an authorization error.\n    guidance: >-\n      Kentico explicitly recommends NOT placing the key in a browser client —\n      proxy GraphQL requests through a backend that adds the Authorization\n      header, because a key sent from a\
  \ public page is visible to anyone.\n    docs: https://docs.kentico.com/documentation/developers-and-admins/configuration/headless-channel-management\n\n  - name: XperiencePortalPAT\n    type: http\n    scheme: bearer\n    parameter_name: Authorization\n    format: \"Bearer <PERSONAL_ACCESS_TOKEN>\"\n    surface: Xperience Portal API (SaaS deployment)\n    host: https://xperience-portal.com\n    scope: per Xperience Portal user; project addressed by PROJECT_GUID in the path\n    roles: >-\n      Uploads to non-production environments and (in extraordinary\n      circumstances) production require the DevOps Engineer or Tenant\n      Administrator role.\n    docs: https://docs.kentico.com/documentation/developers-and-admins/deployment/deploy-to-the-saas-environment\n\n  - name: ManagementApiSecret\n    type: apiKey\n    in: header\n    surface: Management API (preview) + Management MCP server\n    format: shared secret, minimum 32 characters\n    configured_by: >-\n      ManagementApiOptions.Secret\
  \ passed to AddKenticoManagementApi() in\n      Program.cs; supplied to the MCP server as the MANAGEMENT_API_SECRET\n      environment variable.\n    warning: >-\n      Kentico states the management API provides only basic authentication and\n      NO per-operation authorization, and must not be enabled on production or\n      any publicly reachable instance. It is a local-development surface.\n    status: preview\n    docs: https://docs.kentico.com/documentation/developers-and-admins/api/management-api/configure-management-mcp-server\n\n  - name: RestServiceBasic\n    type: http\n    scheme: basic\n    surface: Kentico REST service (Kentico 12/13 line)\n    format: Base64-encoded username:password, or a hash parameter for public endpoints\n    docs: https://docs.kentico.com/k12sp/integrating-3rd-party-systems/kentico-rest-service/authenticating-rest-requests\n\nunauthenticated_surfaces:\n  - name: Kentico Docs MCP server\n    url: https://docs.kentico.com/mcp\n    note: >-\n      Probed\
  \ anonymously on 2026-08-13 — initialize and tools/list both returned\n      200 with no credential and no OAuth challenge. There is no\n      /.well-known/oauth-protected-resource (404).\n\nnot_supported:\n  oauth2: >-\n    No OAuth 2.0 or OpenID Connect surface is documented for any Kentico API.\n    scopes/ is therefore intentionally absent — derive-oauth-scopes.py reported\n    zero oauth2 schemes and zero scopes for this provider.\n  mutual_tls: not documented\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kentico/refs/heads/main/authentication/kentico-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- CMS
- Content Management
- Digital Experience Platform
- GraphQL
- REST
- .NET
- Headless
- E-commerce
- Digital Marketing
- Personalization
---
