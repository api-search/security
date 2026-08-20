---
api_key_in: []
api_specs:
- filename: authenticx-agent-api-openapi.yml
  format: yaml
  label: Authenticx Agent API
  slug: authenticx-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-agent-api-openapi.yml
- filename: authenticx-conversations-api-openapi.yml
  format: yaml
  label: Authenticx Conversations API
  slug: authenticx-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-conversations-api-openapi.yml
- filename: authenticx-evaluations-api-openapi.yml
  format: yaml
  label: Authenticx Evaluations API
  slug: authenticx-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-evaluations-api-openapi.yml
- filename: authenticx-hierarchy-api-openapi.yml
  format: yaml
  label: Authenticx Hierarchy API
  slug: authenticx-hierarchy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-hierarchy-api-openapi.yml
- filename: authenticx-interactions-api-openapi.yml
  format: yaml
  label: Authenticx Interactions API
  slug: authenticx-interactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-interactions-api-openapi.yml
- filename: authenticx-media-api-openapi.yml
  format: yaml
  label: Authenticx Media API
  slug: authenticx-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-media-api-openapi.yml
- filename: authenticx-metadata-api-openapi.yml
  format: yaml
  label: Authenticx Metadata API
  slug: authenticx-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-metadata-api-openapi.yml
- filename: authenticx-modelresults-api-openapi.yml
  format: yaml
  label: Authenticx Model Results API
  slug: authenticx-modelresults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-modelresults-api-openapi.yml
- filename: authenticx-receipts-api-openapi.yml
  format: yaml
  label: Authenticx Receipts API
  slug: authenticx-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-receipts-api-openapi.yml
- filename: authenticx-roles-api-openapi.yml
  format: yaml
  label: Authenticx Roles API
  slug: authenticx-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-roles-api-openapi.yml
- filename: authenticx-scim-resourcetypes-api-openapi.yml
  format: yaml
  label: Authenticx (Scim) ResourceTypes API
  slug: authenticx-scim-resourcetypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-scim-resourcetypes-api-openapi.yml
- filename: authenticx-scim-schemas-api-openapi.yml
  format: yaml
  label: Authenticx (Scim) Schemas API
  slug: authenticx-scim-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-scim-schemas-api-openapi.yml
- filename: authenticx-scim-serviceproviderconfig-api-openapi.yml
  format: yaml
  label: Authenticx (Scim) ServiceProviderConfig API
  slug: authenticx-scim-serviceproviderconfig-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-scim-serviceproviderconfig-api-openapi.yml
- filename: authenticx-scim-users-api-openapi.yml
  format: yaml
  label: Authenticx (Scim) Users API
  slug: authenticx-scim-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-scim-users-api-openapi.yml
- filename: authenticx-textmedia-api-openapi.yml
  format: yaml
  label: Authenticx Text Media API
  slug: authenticx-textmedia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-textmedia-api-openapi.yml
- filename: authenticx-user-api-openapi.yml
  format: yaml
  label: Authenticx User API
  slug: authenticx-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-user-api-openapi.yml
- filename: authenticx-userhierarchy-api-openapi.yml
  format: yaml
  label: Authenticx User Hierarchy API
  slug: authenticx-userhierarchy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-userhierarchy-api-openapi.yml
- filename: authenticx-workflows-api-openapi.yml
  format: yaml
  label: Authenticx Workflows API
  slug: authenticx-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-workflows-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Authenticx Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Authenticx secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Authenticx
provider_slug: authenticx
scheme_count: 1
schemes:
- client_authentication:
  - method: client_secret_post
    note: '`client_id` and `client_secret` in an application/x-www-form-urlencoded body alongside `grant_type=client_credentials&scope=acxapi` (the form shown in the docs).'
  - method: client_secret_basic
    note: 'Base64 `client-id:client-secret` in an `Authorization: Basic` header; grant type and scope still go in the form body. Documented as an accepted alternative.'
  description: 'The only security scheme declared in the AcxAPI OpenAPI. Client credentials are issued by Authenticx during customer onboarding — there is no self-serve developer signup. The resulting bearer token is sent on every request as `Authorization: Bearer <access_token>`.'
  flows:
  - flow: clientCredentials
    scopes:
    - acxapi
    tokenUrl: https://api.beauthenticx.com/connect/token
  name: OAuth2
  sources:
  - openapi/authenticx-acxapi-openapi.yml
  type: oauth2
slug: authenticx-authentication
source_filename: authenticx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: openapi/authenticx-acxapi-openapi.yml\ndocs: https://authenticx.readme.io/reference/retrieving-an-access-token\nadditional_docs:\n- https://authenticx.readme.io/reference/authorizing-requests\n- https://api.beauthenticx.com/.well-known/openid-configuration\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\n  bearer_token: true\n  token_lifetime_seconds: 3600\n  credential_issuance: onboarding\n  self_serve_signup: false\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    The only security scheme declared in the AcxAPI OpenAPI. Client credentials are issued by Authenticx during\n    customer onboarding — there is no self-serve developer signup. The resulting bearer token is sent on every\n    request as `Authorization: Bearer <access_token>`.\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.beauthenticx.com/connect/token\n    scopes:\n\
  \    - acxapi\n  sources:\n  - openapi/authenticx-acxapi-openapi.yml\n  client_authentication:\n  - method: client_secret_post\n    note: >-\n      `client_id` and `client_secret` in an application/x-www-form-urlencoded body alongside\n      `grant_type=client_credentials&scope=acxapi` (the form shown in the docs).\n  - method: client_secret_basic\n    note: >-\n      Base64 `client-id:client-secret` in an `Authorization: Basic` header; grant type and scope still go in the\n      form body. Documented as an accepted alternative.\nenvironments:\n- name: production\n  token_url: https://api.beauthenticx.com/connect/token\n  base_url: https://api.beauthenticx.com\n- name: experimental\n  token_url: https://api.authcx.com/connect/token\n  base_url: https://api.authcx.com\nopenid_connect:\n  discovery: https://api.beauthenticx.com/.well-known/openid-configuration\n  status: 200\n  issuer: https://acxapi-net8d-prod1.azurewebsites.net\n  implementation: Duende IdentityServer (inferred from the\
  \ /connect/* endpoint set)\n  endpoints:\n    authorization: https://acxapi-net8d-prod1.azurewebsites.net/connect/authorize\n    token: https://acxapi-net8d-prod1.azurewebsites.net/connect/token\n    userinfo: https://acxapi-net8d-prod1.azurewebsites.net/connect/userinfo\n    jwks: https://acxapi-net8d-prod1.azurewebsites.net/.well-known/openid-configuration/jwks\n    introspection: https://acxapi-net8d-prod1.azurewebsites.net/connect/introspect\n    revocation: https://acxapi-net8d-prod1.azurewebsites.net/connect/revocation\n    end_session: https://acxapi-net8d-prod1.azurewebsites.net/connect/endsession\n    device_authorization: https://acxapi-net8d-prod1.azurewebsites.net/connect/deviceauthorization\n    pushed_authorization_request: https://acxapi-net8d-prod1.azurewebsites.net/connect/par\n    backchannel_authentication: https://acxapi-net8d-prod1.azurewebsites.net/connect/ciba\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - implicit\n\
  \  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:openid:params:grant-type:ciba\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg_values_supported:\n  - RS256\n  require_pushed_authorization_requests: false\nobservations:\n- >-\n  The discovery document's `issuer` and every advertised endpoint point at the underlying Azure App Service\n  hostname (acxapi-net8d-prod1.azurewebsites.net), not at the public api.beauthenticx.com host that serves the\n  document. A strict OIDC client that follows discovery will therefore be redirected off the branded host, and\n  the token endpoint the docs tell integrators to call (api.beauthenticx.com/connect/token) is NOT the one the\n  discovery document advertises. Worth raising with the provider.\n- >-\n  The OpenAPI declares only the `clientCredentials` flow and only the `acxapi` scope, while the OIDC provider\n  advertises authorization_code, implicit, device_code and CIBA plus\
  \ openid/profile/email/address/roles/\n  offline_access. The extra grants and scopes serve the AcxPlatform web application and the documented\n  \"Authenticx as an Auth Provider\" Salesforce OIDC integration, not AcxAPI machine-to-machine access.\n- >-\n  Access tokens expire after 3600 seconds (documented); the client-credentials flow has no refresh token, so\n  integrators re-request a token.\nx-evidence:\n- url: https://api.beauthenticx.com/swagger/v1/swagger.json\n  http_status: 200\n  fetched: '2026-08-06'\n- url: https://api.beauthenticx.com/.well-known/openid-configuration\n  http_status: 200\n  fetched: '2026-08-06'\n- url: https://authenticx.readme.io/reference/retrieving-an-access-token\n  http_status: 200\n  fetched: '2026-08-06'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/authentication/authenticx-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Conversation Intelligence
- Healthcare
- Speech Analytics
- Contact Center
- Customer Experience
- Quality Assurance
- Pharmacovigilance
- Patient Experience
- Transcription
- Life Sciences
- SCIM
- Authentication
---
