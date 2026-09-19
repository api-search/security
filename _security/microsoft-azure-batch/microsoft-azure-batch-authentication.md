---
anonymous_access: false
api_key_in: []
api_specs:
- filename: microsoft-azure-batch-batch-service-openapi.json
  format: json
  label: Azure Batch Service API
  slug: microsoft-azure-batch-batch-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/_original/microsoft-azure-batch-batch-service-openapi.json
- filename: microsoft-azure-batch-management-openapi.json
  format: json
  label: Azure Batch Management API
  slug: microsoft-azure-batch-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/_original/microsoft-azure-batch-management-openapi.json
- filename: microsoft-azure-batch-jobs-api-openapi.yml
  format: yaml
  label: microsoft-azure-batch Jobs API
  slug: microsoft-azure-batch-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-jobs-api-openapi.yml
- filename: microsoft-azure-batch-pools-api-openapi.yml
  format: yaml
  label: microsoft-azure-batch Pools API
  slug: microsoft-azure-batch-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-pools-api-openapi.yml
- filename: microsoft-azure-batch-tasks-api-openapi.yml
  format: yaml
  label: microsoft-azure-batch Tasks API
  slug: microsoft-azure-batch-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-tasks-api-openapi.yml
auth_types:
- oauth2
- shared-key
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Microsoft Azure Batch Authentication
name_suffix: Authentication
oauth_flows:
- implicit
- authorization_code
- client_credentials
overview: Microsoft Azure Batch secures its APIs with oauth2 and shared-key across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit, authorization_code, and client_credentials flow(s).
provider_name: Microsoft Azure Batch
provider_slug: microsoft-azure-batch
scheme_count: 3
schemes:
- authority: Microsoft Entra ID
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: implicit
    scopes:
      https://batch.core.windows.net//.default: ''
  name: OAuth2Auth
  note: Declared verbatim in the provider contract. The double slash in the scope (batch.core.windows.net//.default) is Microsoft's own spelling, not a typo on our side — the resource URI ends in a slash and ".default" is appended to it.
  plane: data
  resource: https://batch.core.windows.net/
  source: openapi/_original/microsoft-azure-batch-batch-service-openapi.json
  type: oauth2
- authority: Microsoft Entra ID
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes:
      user_impersonation: impersonate your user account
  name: azure_auth
  plane: management
  resource: https://management.azure.com/
  source: openapi/_original/microsoft-azure-batch-management-openapi.json
  type: oauth2
- description: 'Legacy HMAC-SHA256 shared-key authentication using a Batch account access key. Authorization: SharedKey <account-name>:<base64 signature>. Microsoft documents it but recommends Entra ID instead; shared-key auth cannot be scoped, rotated per caller, or audited per identity, and is unavailable in user subscription pool allocation mode for some operations.'
  docs: https://learn.microsoft.com/en-us/rest/api/batchservice/authenticate-requests-to-the-azure-batch-service
  header: Authorization
  in: header
  name: Shared Key
  plane: data
  scheme: SharedKey
  type: apiKey
slug: microsoft-azure-batch-authentication
source_filename: microsoft-azure-batch-authentication.yml
source_heading: Authentication Profile
source_url: openapi/_original/microsoft-azure-batch-batch-service-openapi.json
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: https://learn.microsoft.com/en-us/rest/api/batchservice/authenticate-requests-to-the-azure-batch-service\ndocs: https://learn.microsoft.com/en-us/azure/batch/batch-aad-auth\nupgraded_from:\n  method: derived\n  reason: >-\n    The derived profile read only the three AE-authored tag-split specs in openapi/ and\n    reported a single implicit-flow scheme with the legacy v1.0 authorize endpoint. The\n    provider's own 2025-06-01 contract (openapi/_original/) and the Entra ID provider\n    metadata probed at login.microsoftonline.com give the real picture, below.\nsummary:\n  types:\n    - oauth2\n    - shared-key\n  oauth2_flows:\n    - implicit\n    - authorization_code\n    - client_credentials\n  recommended: Microsoft Entra ID (OAuth 2.0) with a managed identity or service principal\n  planes: 2\nschemes:\n  - name: OAuth2Auth\n    type: oauth2\n    plane: data\n    authority: Microsoft Entra ID\n    flows:\n      - flow:\
  \ implicit\n        authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n        scopes:\n          https://batch.core.windows.net//.default: ''\n    resource: https://batch.core.windows.net/\n    note: >-\n      Declared verbatim in the provider contract. The double slash in the scope\n      (batch.core.windows.net//.default) is Microsoft's own spelling, not a typo on our\n      side — the resource URI ends in a slash and \".default\" is appended to it.\n    source: openapi/_original/microsoft-azure-batch-batch-service-openapi.json\n  - name: azure_auth\n    type: oauth2\n    plane: management\n    authority: Microsoft Entra ID\n    flows:\n      - flow: implicit\n        authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n        scopes:\n          user_impersonation: impersonate your user account\n    resource: https://management.azure.com/\n    source: openapi/_original/microsoft-azure-batch-management-openapi.json\n  - name: Shared\
  \ Key\n    type: apiKey\n    in: header\n    header: Authorization\n    plane: data\n    scheme: SharedKey\n    description: >-\n      Legacy HMAC-SHA256 shared-key authentication using a Batch account access key.\n      Authorization: SharedKey <account-name>:<base64 signature>. Microsoft documents it\n      but recommends Entra ID instead; shared-key auth cannot be scoped, rotated per\n      caller, or audited per identity, and is unavailable in user subscription pool\n      allocation mode for some operations.\n    docs: https://learn.microsoft.com/en-us/rest/api/batchservice/authenticate-requests-to-the-azure-batch-service\nidentity_options:\n  - name: Managed identity\n    description: >-\n      System-assigned or user-assigned managed identity on the calling Azure resource, and\n      separately on the Batch pool itself for access to Key Vault, ACR and Storage.\n    docs: https://learn.microsoft.com/en-us/azure/batch/managed-identity-pools\n  - name: Service principal\n    description:\
  \ App registration in Entra ID with a client secret or certificate; the\n      client-credentials path for unattended Batch clients.\n    docs: https://learn.microsoft.com/en-us/azure/batch/batch-aad-auth\n  - name: User (interactive)\n    description: Interactive sign-in for az batch account login and portal access.\nauthorization_server:\n  issuer_metadata: https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration\n  probed: '2026-09-17'\n  http_status: 200\n  artifact: well-known/microsoft-azure-batch-openid-configuration.json\n  jwks_uri: https://login.microsoftonline.com/common/discovery/v2.0/keys\n  token_endpoint: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  token_endpoint_auth_methods_supported:\n    - client_secret_post\n    - private_key_jwt\n    - client_secret_basic\n    - self_signed_tls_client_auth\nrequest_signing:\n  headers:\n    - name: Authorization\n      required: true\n    - name: ocp-date\n      required: false\n      description:\
  \ >-\n        Present on all 72 data-plane operations. Carries the request time used in the\n        shared-key signature; also accepted alongside Entra tokens.\n    - name: client-request-id\n      required: false\n      description: Caller-supplied correlation id, present on all 72 operations.\n    - name: return-client-request-id\n      required: false\n      description: When true, the service echoes client-request-id back in the response.\nrbac:\n  model: Azure RBAC\n  note: >-\n    Data-plane authorization is Azure RBAC on the Batch account resource. Microsoft\n    publishes Batch-specific built-in roles (for example Azure Batch Data Contributor /\n    Data Reader) rather than OAuth scopes; the only OAuth scope the contract declares is\n    the resource-wide .default. See scopes/microsoft-azure-batch-scopes.yml.\n  docs: https://learn.microsoft.com/en-us/azure/batch/batch-account-create-portal\nsources:\n  - openapi/_original/microsoft-azure-batch-batch-service-openapi.json\n  -\
  \ openapi/_original/microsoft-azure-batch-management-openapi.json\n  - https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration\n  - https://learn.microsoft.com/en-us/azure/batch/batch-aad-auth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/authentication/microsoft-azure-batch-authentication.yml
summary_line: oauth2/shared-key · 3 schemes
tags:
- Batch
- Compute
- Job Scheduling
- High Performance Computing
- Cloud
- Microsoft
- Azure
- Parallel Processing
- Scheduling
- Infrastructure
---
