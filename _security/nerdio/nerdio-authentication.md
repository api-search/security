---
api_key_in:
- header
api_specs:
- filename: nerdio-health-api-openapi.yml
  format: yaml
  label: Nerdio Health API
  slug: nerdio-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nerdio/refs/heads/main/openapi/nerdio-health-api-openapi.yml
- filename: nerdio-install-api-openapi.yml
  format: yaml
  label: Nerdio Install API
  slug: nerdio-install-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nerdio/refs/heads/main/openapi/nerdio-install-api-openapi.yml
- filename: nerdio-invoices-api-openapi.yml
  format: yaml
  label: Nerdio Invoices API
  slug: nerdio-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nerdio/refs/heads/main/openapi/nerdio-invoices-api-openapi.yml
- filename: nerdio-usage-api-openapi.yml
  format: yaml
  label: Nerdio Usage API
  slug: nerdio-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nerdio/refs/heads/main/openapi/nerdio-usage-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Nerdio Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Nerdio secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Nerdio
provider_slug: nerdio
scheme_count: 3
schemes:
- api: Nerdio Manager Distributor API
  description: API key for authentication. Mandatory on every Distributor API endpoint. Issued by Nerdio on request to nmm.support@getnerdio.com along with access to the Mothership licensing portal.
  docs: https://nmmhelp.getnerdio.com/hc/en-us/articles/26125597051277-Nerdio-Manager-Distributor-API-Getting-Started
  in: header
  name: APIKey
  operational_notes:
  - Nerdio states it may apply IP allow-listing in future to further protect the key.
  - A 401 Unauthorized is returned when the key does not authorize the request.
  parameter_name: APIKey
  required: true
  sources:
  - openapi/nerdio-distributor-api-openapi.json
  type: apiKey
- api: Nerdio Manager for Enterprise REST API
  authorization_model: Entra ID app role (RestClient) assigned to the calling application
  credentials:
  - client_id
  - client_secret
  - tenant_id
  docs: https://nmehelp.getnerdio.com/hc/en-us/articles/26124297445901-Getting-Started-with-REST-API-Integration
  flow: clientCredentials
  identity_provider: Microsoft Entra ID
  name: EntraIdClientCredentials
  provisioning: System > Settings > Integrations > REST API. Step 1 creates a new Azure application under the existing nerdio-nmw-app app registration; step 2 grants admin consent for the assigned permissions; step 3 generates the client secret. The application's Application ID URI must be set (api://<app_id>) and the manifest accessTokenAcceptedVersion set to 2.
  scope: api://{nerdio-nmw-app-application-id}/.default
  sources:
  - https://nmehelp.getnerdio.com/hc/en-us/articles/27422824784269-REST-API-Manual-Configuration
  token_url: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  type: oauth2
- api: Nerdio Manager for MSP Partner API
  credentials:
  - client_id
  - client_secret
  - tenant_id
  docs: https://nmmhelp.getnerdio.com/hc/en-us/articles/26125599431693-Nerdio-Manager-Partner-API-Getting-Started
  flow: clientCredentials
  identity_provider: Microsoft Entra ID
  name: EntraIdClientCredentialsMsp
  provisioning: At the MSP level, System > System Settings > Integrations > REST API. Creates a client application under the nerdio-nmm-app app registration, grants admin consent, and generates the client secret. Swagger on the install accepts the client_id/client_secret pair via its Authorize dialog.
  scope: api://{nerdio-nmm-app-application-id}/.default
  token_url: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  type: oauth2
slug: nerdio-authentication
source_filename: nerdio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: openapi/nerdio-distributor-api-openapi.json\ndocs: https://nmehelp.getnerdio.com/hc/en-us/articles/26124297445901-Getting-Started-with-REST-API-Integration\nnotes: >-\n  Nerdio runs two distinct authentication models. The public Distributor API uses a\n  static APIKey request header issued by Nerdio support. The customer-deployed NME\n  and NMM REST APIs use OAuth2 client credentials against Microsoft Entra ID: enabling\n  the API in the product provisions a client application under the nerdio-nmw-app\n  (NME) / nerdio-nmm-app (NMM) app registration in the customer's own tenant, and\n  calls carry a bearer token acquired for the install's Application ID URI with the\n  .default scope. The distributor OpenAPI declares the API key as a required header\n  PARAMETER rather than a components.securitySchemes entry, so the mechanical\n  securityScheme derivation yields nothing; this file is written from the spec\n  parameters plus\
  \ the published docs.\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\n  identity_provider: Microsoft Entra ID (per-customer tenant)\nschemes:\n- name: APIKey\n  type: apiKey\n  in: header\n  parameter_name: APIKey\n  api: Nerdio Manager Distributor API\n  required: true\n  description: >-\n    API key for authentication. Mandatory on every Distributor API endpoint. Issued\n    by Nerdio on request to nmm.support@getnerdio.com along with access to the\n    Mothership licensing portal.\n  sources: [openapi/nerdio-distributor-api-openapi.json]\n  docs: https://nmmhelp.getnerdio.com/hc/en-us/articles/26125597051277-Nerdio-Manager-Distributor-API-Getting-Started\n  operational_notes:\n  - Nerdio states it may apply IP allow-listing in future to further protect the key.\n  - A 401 Unauthorized is returned when the key does not authorize the request.\n- name: EntraIdClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  api: Nerdio Manager\
  \ for Enterprise REST API\n  identity_provider: Microsoft Entra ID\n  token_url: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  scope: api://{nerdio-nmw-app-application-id}/.default\n  credentials:\n  - client_id\n  - client_secret\n  - tenant_id\n  provisioning: >-\n    System > Settings > Integrations > REST API. Step 1 creates a new Azure\n    application under the existing nerdio-nmw-app app registration; step 2 grants\n    admin consent for the assigned permissions; step 3 generates the client secret.\n    The application's Application ID URI must be set (api://<app_id>) and the\n    manifest accessTokenAcceptedVersion set to 2.\n  authorization_model: Entra ID app role (RestClient) assigned to the calling application\n  sources: [https://nmehelp.getnerdio.com/hc/en-us/articles/27422824784269-REST-API-Manual-Configuration]\n  docs: https://nmehelp.getnerdio.com/hc/en-us/articles/26124297445901-Getting-Started-with-REST-API-Integration\n- name: EntraIdClientCredentialsMsp\n\
  \  type: oauth2\n  flow: clientCredentials\n  api: Nerdio Manager for MSP Partner API\n  identity_provider: Microsoft Entra ID\n  token_url: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  scope: api://{nerdio-nmm-app-application-id}/.default\n  credentials:\n  - client_id\n  - client_secret\n  - tenant_id\n  provisioning: >-\n    At the MSP level, System > System Settings > Integrations > REST API. Creates a\n    client application under the nerdio-nmm-app app registration, grants admin\n    consent, and generates the client secret. Swagger on the install accepts the\n    client_id/client_secret pair via its Authorize dialog.\n  docs: https://nmmhelp.getnerdio.com/hc/en-us/articles/26125599431693-Nerdio-Manager-Partner-API-Getting-Started\nscopes:\n  model: >-\n    No published scope catalog. The NME and NMM APIs use the Entra ID application\n    .default scope for the install's own Application ID URI; granular authorization\n    is expressed as Entra app roles and Nerdio\
  \ Manager RBAC roles inside the product,\n    not as OAuth scopes. scopes/ is therefore not emitted for this provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nerdio/refs/heads/main/authentication/nerdio-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Azure Virtual Desktop
- Windows 365
- Virtual Desktop Infrastructure
- Cloud Desktop Management
- Microsoft Intune
- Managed Service Providers
- Cloud Cost Optimization
- Endpoint Management
- IT Automation
---
