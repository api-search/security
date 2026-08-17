---
api_key_in: []
api_specs:
- filename: microsoft-dynamics-365-sales-accounts-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Sales Accounts API
  slug: microsoft-dynamics-365-sales-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/openapi/microsoft-dynamics-365-sales-accounts-api-openapi.yml
- filename: microsoft-dynamics-365-sales-batch-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Sales $batch API
  slug: microsoft-dynamics-365-sales-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/openapi/microsoft-dynamics-365-sales-batch-api-openapi.yml
- filename: microsoft-dynamics-365-sales-contacts-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Sales Contacts API
  slug: microsoft-dynamics-365-sales-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/openapi/microsoft-dynamics-365-sales-contacts-api-openapi.yml
- filename: microsoft-dynamics-365-sales-invoices-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Sales Invoices API
  slug: microsoft-dynamics-365-sales-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/openapi/microsoft-dynamics-365-sales-invoices-api-openapi.yml
- filename: microsoft-dynamics-365-sales-leads-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Sales Leads API
  slug: microsoft-dynamics-365-sales-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/openapi/microsoft-dynamics-365-sales-leads-api-openapi.yml
- filename: microsoft-dynamics-365-sales-opportunities-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Sales Opportunities API
  slug: microsoft-dynamics-365-sales-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/openapi/microsoft-dynamics-365-sales-opportunities-api-openapi.yml
- filename: microsoft-dynamics-365-sales-products-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Sales Products API
  slug: microsoft-dynamics-365-sales-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/openapi/microsoft-dynamics-365-sales-products-api-openapi.yml
- filename: microsoft-dynamics-365-sales-quotes-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Sales Quotes API
  slug: microsoft-dynamics-365-sales-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/openapi/microsoft-dynamics-365-sales-quotes-api-openapi.yml
- filename: microsoft-dynamics-365-sales-salesorders-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Sales SalesOrders API
  slug: microsoft-dynamics-365-sales-salesorders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/openapi/microsoft-dynamics-365-sales-salesorders-api-openapi.yml
- filename: microsoft-dynamics-365-sales-tasks-api-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Sales Tasks API
  slug: microsoft-dynamics-365-sales-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/openapi/microsoft-dynamics-365-sales-tasks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Microsoft Dynamics 365 Sales Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft Dynamics 365 Sales secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft Dynamics 365 Sales
provider_slug: microsoft-dynamics-365-sales
scheme_count: 1
schemes:
- description: Microsoft Entra ID OAuth 2.0 bearer token
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    client_type: public
    flow: authorizationCode
    scope: '{environment-url}/user_impersonation'
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - client_type: confidential
    flow: clientCredentials
    scope: '{environment-url}/.default'
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/_original/microsoft-dynamics-365-sales-openapi.yml
  type: oauth2
slug: microsoft-dynamics-365-sales-authentication
source_filename: microsoft-dynamics-365-sales-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/microsoft-dynamics-365-sales-openapi.yml\ndocs: https://learn.microsoft.com/en-us/power-apps/developer/data-platform/authenticate-oauth\ndocs_additional:\n- https://learn.microsoft.com/en-us/power-apps/developer/data-platform/authentication\n- https://learn.microsoft.com/en-us/power-apps/developer/data-platform/walkthrough-register-app-azure-active-directory\n- https://learn.microsoft.com/en-us/power-platform/admin/manage-application-users\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials]\n  identity_provider: Microsoft Entra ID\n  transport: 'Authorization: Bearer <access token>'\n  statement: >-\n    Learn, verbatim — \"Client applications must support the use of OAuth to access data by\n    using the Web API.\" There is no API-key, basic-auth or legacy option; the Office365\n    authentication type is deprecated.\n\nschemes:\n- name: oauth2\n  type: oauth2\n\
  \  description: Microsoft Entra ID OAuth 2.0 bearer token\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n    scope: '{environment-url}/user_impersonation'\n    client_type: public\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n    scope: '{environment-url}/.default'\n    client_type: confidential\n  sources:\n  - openapi/_original/microsoft-dynamics-365-sales-openapi.yml\n\ndiscovery:\n  openid_configuration: https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration\n  probed_status: 200\n  saved: well-known/microsoft-dynamics-365-sales-openid-configuration.json\n  issuer: 'https://login.microsoftonline.com/{tenantid}/v2.0'\n  oauth_authorization_server_metadata: 404\n  note: >-\n    The OIDC discovery document is served; RFC 8414\
  \ /.well-known/oauth-authorization-server\n    is not.\n\nregistration:\n  required: true\n  where: Microsoft Entra ID tenant\n  app_types:\n  - type: Web app / API\n    subtypes: [web client, user-agent-based client (SPA)]\n    requires: Sign-On URL\n  - type: Native\n    requires: 'Redirect URI, typically app://<guid>'\n  delegated_permission: Access Dynamics 365 as organization users\n  docs: https://learn.microsoft.com/en-us/power-apps/developer/data-platform/walkthrough-register-app-azure-active-directory\n\nserver_to_server:\n  supported: true\n  mechanism: application user bound to an Entra app registration\n  credentials: [client secret, X.509 certificate]\n  licence: 'does not consume a paid user licence'\n  requires:\n  - a registered Entra app\n  - a Dataverse application user bound to it\n  - a custom security role assigned to that user\n  note: >-\n    Learn, verbatim — \"While you could achieve these scenarios by using credentials for an\n    ordinary user, that user account\
  \ needs a paid license. Don't use this approach.\"\n\ntoken:\n  lifetime: 'approximately 60 minutes (default)'\n  refresh: handled by MSAL token cache; re-acquire per request via a DelegatingHandler\n  library: Microsoft Authentication Library (MSAL)\n  deprecated_library: ADAL — 'isn''t actively receiving updates and is supported only until June 2022'\n\nclient_handling:\n- client: Microsoft.PowerPlatform.Dataverse.Client ServiceClient\n  auth_library: MSAL\n  note: recommended; also handles 429 Retry-After automatically\n- client: Microsoft.Xrm.Tooling.Connector CrmServiceClient\n  auth_library: ADAL\n  note: legacy\n- client: PowerPlatform-Dataverse-Client (Python)\n  auth_library: azure-identity TokenCredential (InteractiveBrowserCredential, ClientSecretCredential, CertificateCredential, AzureCliCredential)\n\nimpersonation:\n  header: CallerObjectId\n  value: Microsoft Entra ID Object ID of the user to impersonate\n  requires: caller holds the impersonation privilege\n  docs: https://learn.microsoft.com/en-us/power-apps/developer/data-platform/webapi/impersonate-another-user-web-api\n\
  \nauthorization_note: >-\n  A valid token is necessary but not sufficient. Effective access is decided by the\n  Dataverse security model — security roles, table and column privileges, privilege depth.\n  See scopes/microsoft-dynamics-365-sales-scopes.yml.\n\nfailure_modes:\n  401:\n  - BadAuthTicket\n  - ExpiredAuthTicket\n  - InsufficientAuthTicket\n  - InvalidAuthTicket\n  - InvalidUserAuth\n  - RequestIsNotAuthenticated\n  - TamperedAuthTicket\n  403:\n  - AccessDenied\n  - PrivilegeDenied\n  - PrincipalPrivilegeDenied\n  - CannotActOnBehalfOfAnotherUser\n  see: errors/microsoft-dynamics-365-sales-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/authentication/microsoft-dynamics-365-sales-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- CRM
- Sales
- Customer Relationship Management
- Dynamics 365
- Microsoft
- Dataverse
- OData
- Sales Automation
---
