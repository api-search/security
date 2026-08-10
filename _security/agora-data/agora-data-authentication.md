---
api_key_in:
- header
- query
api_specs:
- filename: agora-data-health-api-openapi.yml
  format: yaml
  label: Agora Data Health API
  slug: agora-data-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-health-api-openapi.yml
- filename: agora-data-hooks-api-openapi.yml
  format: yaml
  label: Agora Data Hooks API
  slug: agora-data-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-hooks-api-openapi.yml
- filename: agora-data-import-api-openapi.yml
  format: yaml
  label: Agora Data Import API
  slug: agora-data-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-import-api-openapi.yml
- filename: agora-data-inventory-api-openapi.yml
  format: yaml
  label: Agora Data Inventory API
  slug: agora-data-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-inventory-api-openapi.yml
- filename: agora-data-loans-api-openapi.yml
  format: yaml
  label: Agora Data Loans API
  slug: agora-data-loans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-loans-api-openapi.yml
- filename: agora-data-login-api-openapi.yml
  format: yaml
  label: Agora Data Login API
  slug: agora-data-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-login-api-openapi.yml
- filename: agora-data-oauth-api-openapi.yml
  format: yaml
  label: Agora Data OAUTH API
  slug: agora-data-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-oauth-api-openapi.yml
- filename: agora-data-providers-api-openapi.yml
  format: yaml
  label: Agora Data Providers API
  slug: agora-data-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-providers-api-openapi.yml
- filename: agora-data-status-api-openapi.yml
  format: yaml
  label: Agora Data Status API
  slug: agora-data-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-status-api-openapi.yml
- filename: agora-data-uploads-api-openapi.yml
  format: yaml
  label: Agora Data Uploads API
  slug: agora-data-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-uploads-api-openapi.yml
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Agora Data Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Agora Data secures its APIs with apiKey, oauth2, and openIdConnect across 7 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Agora Data
provider_slug: agora-data
scheme_count: 7
schemes:
- applies_to:
  - /api/v1/import
  - /api/v1/import/{dms_vendor}
  - /api/v1/import/{dms_vendor}/{upload_subtype}
  - /api/v1/import/priority/{dms_vendor}/{upload_subtype}
  - /api/v1/uploads/{api_activity_uuid}
  - /api/v1/loans
  - /api/v1/loans/{rest_of_path}
  description: The /api/v1/* loan and import operations require an API key. The live API rejects unauthenticated calls with HTTP 400 {"detail":"Api Key is required"}. The header name is not published in the OpenAPI or on any public page.
  evidence:
    body: '{"detail":"Api Key is required"}'
    http_status: 400
    url: https://api.agoradata.com/api/v1/loans
  in: header
  name: api-key
  type: apiKey
- applies_to:
  - /providers
  - /providers/{provider_name}/{rest_of_path}
  description: The /providers passthrough surface requires an Authorization header. The live API rejects unauthenticated calls with HTTP 400 {"detail":"Authorization header is required"}. The token is issued by the API's own /oauth/token endpoint, which returns an AccessTokenResponse / TokenRequestResponse carrying access_token, token_type, refresh_token, expires_in and scope.
  evidence:
    body: '{"detail":"Authorization header is required"}'
    http_status: 400
    url: https://api.agoradata.com/providers
  name: authorization-header
  scheme: bearer
  type: http
- description: The API hosts its own OAuth authorization-code endpoints. POST /oauth/authorize takes a ClientIdBody {client_id} and returns an AuthCodeResponse {code, redirect_url}; POST /oauth/token rotates tokens and returns {access_token, token_type, refresh_token, expires_in, scope}.
  flows:
  - authorizationUrl: https://api.agoradata.com/oauth/authorize
    flow: authorizationCode
    refresh: true
    tokenUrl: https://api.agoradata.com/oauth/token
  name: oauth2
  operations:
  - create_a_code_oauth_authorize_post
  - rotate_tokens_oauth_token_post
  type: oauth2
- description: POST /login/authenticate accepts a UsernamePassword body {email, password}. A direct resource-owner credential exchange, not part of the OAuth flow above.
  name: password-login
  operations:
  - login_login_authenticate_post
  scheme: basic-json
  type: http
- description: 'The inbound file-delivery webhook receivers (/hooks/files/idms, /hooks/files/autoMaster) authenticate the caller with an x-agora-files-key header. Declared in the OpenAPI as an OPTIONAL header parameter (required: false), which is a security-relevant spec defect — a shared-secret webhook verifier should be required.'
  in: header
  name: webhook-shared-secret
  operations:
  - idms_file_endpoint_hooks_files_idms_post
  - auto_master_file_endpoint_hooks_files_autoMaster_post
  parameter_name: x-agora-files-key
  type: apiKey
- description: GET /inventory/homenet/aggregation takes a REQUIRED api_token query-string parameter. Credentials in the query string are logged by proxies and browsers; this is the weakest of the credential placements on this API.
  in: query
  name: api-token-query
  operations:
  - run_inventory_aggregator_inventory_homenet_aggregation_get
  parameter_name: api_token
  type: apiKey
- description: AgoraPortal (the originator-facing console) authenticates against an Auth0 tenant using OIDC authorization code with PKCE (S256), requesting scopes "openid profile email offline_access" for the "dealer-portal" audience. This governs the portal, not the loan-import API above.
  evidence:
    http_status: 302
    redirects_to: https://agora-data.us.auth0.com/authorize
    url: https://portal.agoradata.com/
  issuer: https://agora-data.us.auth0.com/
  name: openIdConnect
  openIdConnectUrl: https://agora-data.us.auth0.com/.well-known/openid-configuration
  type: openIdConnect
slug: agora-data-authentication
source_filename: agora-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: >-\n  openapi/agora-data-openapi-original.json (auth operations + header/query parameters),\n  live unauthenticated probes of api.agoradata.com, and the Auth0 tenant OIDC discovery\n  document at well-known/agora-data-openid-configuration.json\nnotes: >-\n  The published OpenAPI declares NO components.securitySchemes and no security[] on any\n  operation, so the machine-readable contract does not describe how to authenticate.\n  The auth model below is reconstructed from the auth operations the spec does expose,\n  the header/query parameters it declares, and the error bodies the live API returns to\n  unauthenticated callers. This is a real gap in the provider's spec, not in the API.\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [header, query]\n  oauth2_flows: [authorizationCode, refreshToken]\n  declared_in_openapi: false\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  description: >-\n   \
  \ The /api/v1/* loan and import operations require an API key. The live API rejects\n    unauthenticated calls with HTTP 400 {\"detail\":\"Api Key is required\"}. The header name\n    is not published in the OpenAPI or on any public page.\n  applies_to:\n  - /api/v1/import\n  - /api/v1/import/{dms_vendor}\n  - /api/v1/import/{dms_vendor}/{upload_subtype}\n  - /api/v1/import/priority/{dms_vendor}/{upload_subtype}\n  - /api/v1/uploads/{api_activity_uuid}\n  - /api/v1/loans\n  - /api/v1/loans/{rest_of_path}\n  evidence:\n    url: https://api.agoradata.com/api/v1/loans\n    http_status: 400\n    body: '{\"detail\":\"Api Key is required\"}'\n- name: authorization-header\n  type: http\n  scheme: bearer\n  description: >-\n    The /providers passthrough surface requires an Authorization header. The live API\n    rejects unauthenticated calls with HTTP 400\n    {\"detail\":\"Authorization header is required\"}. The token is issued by the API's own\n    /oauth/token endpoint, which returns an AccessTokenResponse\
  \ / TokenRequestResponse\n    carrying access_token, token_type, refresh_token, expires_in and scope.\n  applies_to:\n  - /providers\n  - /providers/{provider_name}/{rest_of_path}\n  evidence:\n    url: https://api.agoradata.com/providers\n    http_status: 400\n    body: '{\"detail\":\"Authorization header is required\"}'\n- name: oauth2\n  type: oauth2\n  description: >-\n    The API hosts its own OAuth authorization-code endpoints. POST /oauth/authorize takes a\n    ClientIdBody {client_id} and returns an AuthCodeResponse {code, redirect_url};\n    POST /oauth/token rotates tokens and returns {access_token, token_type, refresh_token,\n    expires_in, scope}.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.agoradata.com/oauth/authorize\n    tokenUrl: https://api.agoradata.com/oauth/token\n    refresh: true\n  operations: [create_a_code_oauth_authorize_post, rotate_tokens_oauth_token_post]\n- name: password-login\n  type: http\n  scheme: basic-json\n  description:\
  \ >-\n    POST /login/authenticate accepts a UsernamePassword body {email, password}. A direct\n    resource-owner credential exchange, not part of the OAuth flow above.\n  operations: [login_login_authenticate_post]\n- name: webhook-shared-secret\n  type: apiKey\n  in: header\n  parameter_name: x-agora-files-key\n  description: >-\n    The inbound file-delivery webhook receivers (/hooks/files/idms, /hooks/files/autoMaster)\n    authenticate the caller with an x-agora-files-key header. Declared in the OpenAPI as an\n    OPTIONAL header parameter (required: false), which is a security-relevant spec defect —\n    a shared-secret webhook verifier should be required.\n  operations: [idms_file_endpoint_hooks_files_idms_post, auto_master_file_endpoint_hooks_files_autoMaster_post]\n- name: api-token-query\n  type: apiKey\n  in: query\n  parameter_name: api_token\n  description: >-\n    GET /inventory/homenet/aggregation takes a REQUIRED api_token query-string parameter.\n    Credentials in the\
  \ query string are logged by proxies and browsers; this is the weakest\n    of the credential placements on this API.\n  operations: [run_inventory_aggregator_inventory_homenet_aggregation_get]\n- name: openIdConnect\n  type: openIdConnect\n  description: >-\n    AgoraPortal (the originator-facing console) authenticates against an Auth0 tenant using\n    OIDC authorization code with PKCE (S256), requesting scopes\n    \"openid profile email offline_access\" for the \"dealer-portal\" audience. This governs the\n    portal, not the loan-import API above.\n  openIdConnectUrl: https://agora-data.us.auth0.com/.well-known/openid-configuration\n  issuer: https://agora-data.us.auth0.com/\n  evidence:\n    url: https://portal.agoradata.com/\n    http_status: 302\n    redirects_to: https://agora-data.us.auth0.com/authorize\nunauthenticated_operations:\n- operation: status_endpoint_health_get\n  path: /health\n  note: returns \"ok\" with HTTP 200 anonymously\ngaps:\n- No components.securitySchemes\
  \ in the published OpenAPI, so no operation declares security[].\n- The API-key header name is not published anywhere public.\n- x-agora-files-key is declared optional on both webhook receivers.\n- api_token is passed in the query string on /inventory/homenet/aggregation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/authentication/agora-data-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 7 schemes
tags:
- Company
- Auto Finance
- Automotive
- Lending
- Financial Services
- Fintech
- Loan Origination
- Data Analytics
- Artificial Intelligence
- Capital Markets
---
