---
anonymous_access: false
api_key_in: []
api_specs:
- filename: microsoft-power-platform-metadata-api-openapi.yml
  format: yaml
  label: Microsoft Power Platform Metadata API
  slug: microsoft-power-platform-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-platform/refs/heads/main/openapi/microsoft-power-platform-metadata-api-openapi.yml
- filename: microsoft-power-platform-records-api-openapi.yml
  format: yaml
  label: Microsoft Power Platform Records API
  slug: microsoft-power-platform-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-platform/refs/heads/main/openapi/microsoft-power-platform-records-api-openapi.yml
- filename: microsoft-power-platform-enterprise-policies-openapi.json
  format: json
  label: Power Platform Enterprise Policies (Azure Resource Manager)
  slug: microsoft-power-platform-enterprise-policies
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-platform/refs/heads/main/openapi/_original/microsoft-power-platform-enterprise-policies-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Microsoft Power Platform Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
overview: Microsoft Power Platform secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and implicit flow(s).
provider_name: Microsoft Power Platform
provider_slug: microsoft-power-platform
scheme_count: 2
schemes:
- applies_to:
  - Microsoft Dataverse Web API
  - Power Platform API
  audiences:
  - resource: Dataverse
    scope: https://{org}.api.crm.dynamics.com/.default
  - resource: Power Platform API
    scope: https://api.powerplatform.com/.default
  - note: Delegated permission; the client app id must also be allow-listed per environment.
    resource: Dataverse MCP server
    scope: Dynamics CRM mcp.tools
  description: Microsoft Entra ID OAuth 2.0. The token audience is the resource being called, not a shared Power Platform audience.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
    use: interactive user / delegated access
  - flow: clientCredentials
    note: For Dataverse a service principal also needs a matching APPLICATION USER inside the environment with a security role. A valid token alone is not access.
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
    use: service principal / application user
  name: oauth2
  provider: Microsoft Entra ID (formerly Azure AD)
  sources:
  - openapi/microsoft-power-platform-metadata-api-openapi.yml
  - openapi/microsoft-power-platform-records-api-openapi.yml
  type: oauth2
- applies_to:
  - Power Platform Enterprise Policies (Azure Resource Manager)
  description: Declared verbatim in Microsoft's own Swagger for the Microsoft.PowerPlatform resource provider. Standard Azure Resource Manager auth against the management.azure.com audience.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes:
      user_impersonation: impersonate your user account
  name: azure_auth
  provider: Microsoft Entra ID
  sources:
  - openapi/_original/microsoft-power-platform-enterprise-policies-openapi.json
  type: oauth2
slug: microsoft-power-platform-authentication
source_filename: microsoft-power-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: >-\n  https://learn.microsoft.com/en-us/power-platform/admin/programmability-authentication-v2 and\n  https://learn.microsoft.com/en-us/power-platform/admin/programmability-permission-reference\n  (both HTTP 200, fetched 2026-09-06), reconciled with the securitySchemes derived from\n  openapi/microsoft-power-platform-metadata-api-openapi.yml,\n  openapi/microsoft-power-platform-records-api-openapi.yml and\n  openapi/_original/microsoft-power-platform-enterprise-policies-openapi.json\ndocs: https://learn.microsoft.com/en-us/power-platform/admin/programmability-authentication-v2\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  api_keys: false\n  api_key_note: >-\n    There are no API keys anywhere in the Power Platform surface. Every call on every host is a\n    Microsoft Entra ID bearer token, which is why there is no test/live key prefix in sandbox/.\nschemes:\n\
  - name: oauth2\n  type: oauth2\n  applies_to:\n  - Microsoft Dataverse Web API\n  - Power Platform API\n  provider: Microsoft Entra ID (formerly Azure AD)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    use: interactive user / delegated access\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n    use: service principal / application user\n    note: >-\n      For Dataverse a service principal also needs a matching APPLICATION USER inside the\n      environment with a security role. A valid token alone is not access.\n  description: >-\n    Microsoft Entra ID OAuth 2.0. The token audience is the resource being called, not a shared\n    Power Platform audience.\n  audiences:\n  - resource: Dataverse\n    scope: https://{org}.api.crm.dynamics.com/.default\n  - resource: Power Platform\
  \ API\n    scope: https://api.powerplatform.com/.default\n  - resource: Dataverse MCP server\n    scope: Dynamics CRM mcp.tools\n    note: Delegated permission; the client app id must also be allow-listed per environment.\n  sources:\n  - openapi/microsoft-power-platform-metadata-api-openapi.yml\n  - openapi/microsoft-power-platform-records-api-openapi.yml\n- name: azure_auth\n  type: oauth2\n  applies_to:\n  - Power Platform Enterprise Policies (Azure Resource Manager)\n  provider: Microsoft Entra ID\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes:\n      user_impersonation: impersonate your user account\n  description: >-\n    Declared verbatim in Microsoft's own Swagger for the Microsoft.PowerPlatform resource\n    provider. Standard Azure Resource Manager auth against the management.azure.com audience.\n  sources:\n  - openapi/_original/microsoft-power-platform-enterprise-policies-openapi.json\noidc:\n  discovery:\
  \ https://login.microsoftonline.com/{tenant}/v2.0/.well-known/openid-configuration\n  note: >-\n    No Power Platform host serves its own openid-configuration - the identity plane is Entra ID.\n    See well-known/microsoft-power-platform-well-known.yml.\nauthorization:\n  model: >-\n    Two independent layers. Entra ID decides whether the caller may reach the API; Dataverse\n    security roles and Power Platform admin permissions decide what the caller may do once in.\n    A 403 means the second layer refused and no retry will help.\n  reference: https://learn.microsoft.com/en-us/power-platform/admin/programmability-permission-reference\nobserved:\n- url: https://api.powerplatform.com/licensing/billingPolicies?api-version=2022-03-01-preview\n  status: 401\n  www_authenticate: Bearer error=\"invalid_token\"\n  probed: '2026-09-06'\n- url: https://api.bap.microsoft.com/.well-known/security.txt\n  status: 401\n  probed: '2026-09-06'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-platform/refs/heads/main/authentication/microsoft-power-platform-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Dataverse
- Low-Code
- Microsoft
- Power Apps
- Power Automate
- Power BI
---
