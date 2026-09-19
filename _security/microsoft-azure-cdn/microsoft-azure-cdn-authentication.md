---
anonymous_access: false
api_key_in: []
api_specs:
- filename: microsoft-azure-cdn-management-openapi.json
  format: json
  label: Azure CDN Management API (Microsoft.Cdn)
  slug: microsoft-azure-cdn-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cdn/refs/heads/main/openapi/microsoft-azure-cdn-management-openapi.json
- filename: microsoft-azure-cdn-operations-api-openapi.yml
  format: yaml
  label: microsoft-azure-cdn Operations API
  slug: microsoft-azure-cdn-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cdn/refs/heads/main/openapi/microsoft-azure-cdn-operations-api-openapi.yml
- filename: microsoft-azure-cdn-profiles-api-openapi.yml
  format: yaml
  label: microsoft-azure-cdn Profiles API
  slug: microsoft-azure-cdn-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cdn/refs/heads/main/openapi/microsoft-azure-cdn-profiles-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Microsoft Azure Cdn Authentication
name_suffix: Authentication
oauth_flows:
- implicit
- client_credentials
- authorization_code
overview: Microsoft Azure Cdn secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit, client_credentials, and authorization_code flow(s).
provider_name: Microsoft Azure Cdn
provider_slug: microsoft-azure-cdn
scheme_count: 1
schemes:
- applied_to: all 115 operations, via the contract's global security block
  description: Azure Active Directory (Microsoft Entra ID) OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    declared_in: contract
    flow: implicit
    scopes: 1
  - declared_in: authorization server discovery + docs
    flow: client_credentials
    scope: https://management.azure.com/.default
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    declared_in: authorization server discovery
    flow: authorization_code
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  header: 'Authorization: Bearer <token>'
  in: header
  name: azure_auth
  sources:
  - openapi/microsoft-azure-cdn-management-openapi.json
  type: oauth2
slug: microsoft-azure-cdn-authentication
source_filename: microsoft-azure-cdn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: >-\n  openapi/microsoft-azure-cdn-management-openapi.json (securityDefinitions),\n  well-known/microsoft-azure-cdn-openid-configuration.json (live fetch 2026-09-17),\n  https://learn.microsoft.com/en-us/rest/api/azure/,\n  https://learn.microsoft.com/en-us/azure/role-based-access-control/built-in-roles/networking\ndocs: https://learn.microsoft.com/en-us/rest/api/azure/\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\n  - client_credentials\n  - authorization_code\n  api_keys: false\n  mutual_tls: false\n  note: >-\n    The contract declares only the implicit flow, which is the legacy Swagger 2.0 representation Azure\n    has used since 2015 and is NOT how the API is actually called. The authorization server's own\n    discovery document (fetched live) advertises authorization_code, client_credentials, device_code and\n    refresh_token; the documented path for a service integration is client_credentials against\n\
  \    https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token with scope\n    https://management.azure.com/.default. Recorded here because a client generated straight from the\n    spec would implement the wrong flow.\nschemes:\n- name: azure_auth\n  type: oauth2\n  in: header\n  header: 'Authorization: Bearer <token>'\n  description: Azure Active Directory (Microsoft Entra ID) OAuth2 Flow.\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n    declared_in: contract\n  - flow: client_credentials\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n    scope: https://management.azure.com/.default\n    declared_in: authorization server discovery + docs\n  - flow: authorization_code\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    declared_in: authorization server discovery\n\
  \  applied_to: all 115 operations, via the contract's global security block\n  sources:\n  - openapi/microsoft-azure-cdn-management-openapi.json\nauthorization_server:\n  issuer: https://login.microsoftonline.com/{tenantid}/v2.0\n  discovery: https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration\n  discovery_http_status: 200\n  discovery_file: well-known/microsoft-azure-cdn-openid-configuration.json\n  authorization_endpoint: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n  token_endpoint: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  jwks_uri: https://login.microsoftonline.com/common/discovery/v2.0/keys\n  oidc_scopes: [openid, profile, email, offline_access]\naudience: https://management.azure.com/\nidentity_types:\n- name: User principal\n  note: Interactive sign-in; az login or the portal.\n- name: Service principal (app registration)\n  note: Client credentials with a secret or certificate. The standard non-interactive integration.\n\
  - name: Managed identity\n  note: >-\n    System- or user-assigned identity on an Azure resource; no secret to store. The recommended posture\n    for an agent running inside Azure.\nauthorization_model:\n  style: Azure RBAC role assignment, evaluated per ARM resource scope\n  note: >-\n    OAuth scope alone grants nothing here. The token carries the coarse\n    https://management.azure.com/.default scope; what a caller may actually do is decided by RBAC role\n    assignments on the subscription, resource group or individual profile. See\n    scopes/microsoft-azure-cdn-scopes.yml.\n  docs: https://learn.microsoft.com/en-us/azure/role-based-access-control/built-in-roles/networking\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cdn/refs/heads/main/authentication/microsoft-azure-cdn-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- CDN
- Edge
- Caching
- Cloud Infrastructure
- Networking
- Web Performance
- Azure
- Content Delivery
- Web Application Firewall
---
