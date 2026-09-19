---
anonymous_access: false
api_key_in: []
api_specs:
- filename: seismic-content-analytics-api-openapi.yml
  format: yaml
  label: Seismic Content Analytics API
  slug: seismic-content-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-content-analytics-api-openapi.yml
- filename: seismic-content-api-openapi.yml
  format: yaml
  label: Seismic Content API
  slug: seismic-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-content-api-openapi.yml
- filename: seismic-content-profiles-api-openapi.yml
  format: yaml
  label: Seismic Content Profiles API
  slug: seismic-content-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-content-profiles-api-openapi.yml
- filename: seismic-content-properties-api-openapi.yml
  format: yaml
  label: Seismic Content Properties API
  slug: seismic-content-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-content-properties-api-openapi.yml
- filename: seismic-data-sources-api-openapi.yml
  format: yaml
  label: Seismic Data Sources API
  slug: seismic-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-data-sources-api-openapi.yml
- filename: seismic-delivery-analytics-api-openapi.yml
  format: yaml
  label: Seismic Delivery Analytics API
  slug: seismic-delivery-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-delivery-analytics-api-openapi.yml
- filename: seismic-delivery-api-openapi.yml
  format: yaml
  label: Seismic Delivery API
  slug: seismic-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-delivery-api-openapi.yml
- filename: seismic-folders-api-openapi.yml
  format: yaml
  label: Seismic Folders API
  slug: seismic-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-folders-api-openapi.yml
- filename: seismic-generation-jobs-api-openapi.yml
  format: yaml
  label: Seismic Generation Jobs API
  slug: seismic-generation-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-generation-jobs-api-openapi.yml
- filename: seismic-groups-api-openapi.yml
  format: yaml
  label: Seismic Groups API
  slug: seismic-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-groups-api-openapi.yml
- filename: seismic-livedocs-api-openapi.yml
  format: yaml
  label: Seismic LiveDocs API
  slug: seismic-livedocs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-livedocs-api-openapi.yml
- filename: seismic-reports-api-openapi.yml
  format: yaml
  label: Seismic Reports API
  slug: seismic-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-reports-api-openapi.yml
- filename: seismic-roles-api-openapi.yml
  format: yaml
  label: Seismic Roles API
  slug: seismic-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-roles-api-openapi.yml
- filename: seismic-teams-api-openapi.yml
  format: yaml
  label: Seismic Teams API
  slug: seismic-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-teams-api-openapi.yml
- filename: seismic-templates-api-openapi.yml
  format: yaml
  label: Seismic Templates API
  slug: seismic-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-templates-api-openapi.yml
- filename: seismic-user-analytics-api-openapi.yml
  format: yaml
  label: Seismic User Analytics API
  slug: seismic-user-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-user-analytics-api-openapi.yml
- filename: seismic-users-api-openapi.yml
  format: yaml
  label: Seismic Users API
  slug: seismic-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-users-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
- http
description: Seismic authenticates with OAuth 2.0 / OpenID Connect against its own authorization server at https://auth.seismic.com. The OpenAPI documents in this repo declare only a generic HTTP bearer scheme, which understates the model considerably; the authorization server's anonymous discovery document is the authoritative description and is saved verbatim in well-known/.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Seismic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Seismic secures its APIs with oauth2, openIdConnect, and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Seismic
provider_slug: seismic
scheme_count: 3
schemes:
- client_auth:
  - client_secret_basic
  - client_secret_post
  flows:
  - docs: https://developer.seismic.com/seismicsoftware/reference/auth-client-credentials
    grant: client_credentials
    use: Server-to-server integrations acting as the application.
  - docs: https://developer.seismic.com/seismicsoftware/reference/authorization-code-login
    grant: authorization_code
    use: User-delegated access. Required for the MCP server, which accepts user access tokens only.
  - docs: https://developer.seismic.com/seismicsoftware/reference/pkce-get-the-users-authorization-code
    grant: authorization_code + PKCE
    pkce: S256
    use: Public clients.
  - docs: https://developer.seismic.com/seismicsoftware/reference/exchange-the-refresh-token-for-an-access-refresh-token
    grant: refresh_token
  - grant: urn:ietf:params:oauth:grant-type:device_code
  - grant: urn:ietf:params:oauth:grant-type:token-exchange
  - docs: https://developer.seismic.com/seismicsoftware/reference/get-a-token-using-username-and-password
    grant: password
    note: Advertised by the authorization server and documented for token acquisition; not recommended for new integrations.
  name: oauth2
  scopes: scopes/seismic-scopes.yml
  scopes_advertised: 389
  scopes_documented: 39
  type: oauth2
- claims:
  - sub
  - email
  - email_verified
  - name
  - family_name
  - given_name
  - preferred_username
  - profile
  - picture
  - locale
  - updated_at
  docs: https://developer.seismic.com/seismicsoftware/reference/get-open-id-configuration
  name: openIdConnect
  openIdConnectUrl: https://auth.seismic.com/.well-known/openid-configuration
  type: openIdConnect
- bearerFormat: JWT
  description: 'How the token is presented on every call — Authorization: Bearer <access_token>. This is the only scheme declared in the OpenAPI documents; it describes transport, not the OAuth model above.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/seismic-content-api-openapi.yml
  - openapi/seismic-users-api-openapi.yml
  - and 15 further openapi/ documents
  type: http
slug: seismic-authentication
source_filename: seismic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: >-\n  https://developer.seismic.com/seismicsoftware/docs/authentication ,\n  https://developer.seismic.com/seismicsoftware/reference/authentication-overview ,\n  https://auth.seismic.com/.well-known/openid-configuration (probed 2026-09-17, HTTP 200),\n  https://mcp.seismic.com/.well-known/oauth-protected-resource , and openapi/*.yml\ndocs: https://developer.seismic.com/seismicsoftware/docs/authentication\ndescription: >-\n  Seismic authenticates with OAuth 2.0 / OpenID Connect against its own authorization server at\n  https://auth.seismic.com. The OpenAPI documents in this repo declare only a generic HTTP bearer\n  scheme, which understates the model considerably; the authorization server's anonymous discovery\n  document is the authoritative description and is saved verbatim in well-known/.\nsummary:\n  types: [oauth2, openIdConnect, http]\n  primary: oauth2\n  multi_tenant: true\nauthorization_server:\n  issuer: https://auth.seismic.com\n\
  \  discovery: https://auth.seismic.com/.well-known/openid-configuration\n  artifact: well-known/seismic-auth-openid-configuration.json\n  probed: '2026-09-17'\n  http_status: 200\n  authorization_endpoint: https://auth.seismic.com/connect/authorize\n  token_endpoint: https://auth.seismic.com/connect/token\n  userinfo_endpoint: https://auth.seismic.com/connect/userinfo\n  introspection_endpoint: https://auth.seismic.com/connect/introspect\n  revocation_endpoint: https://auth.seismic.com/connect/revocation\n  end_session_endpoint: https://auth.seismic.com/connect/endsession\n  jwks_uri: https://auth.seismic.com/.well-known/openid-configuration/jwks\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - grant: client_credentials\n    docs: https://developer.seismic.com/seismicsoftware/reference/auth-client-credentials\n    use: Server-to-server integrations acting as the application.\n  - grant: authorization_code\n    docs: https://developer.seismic.com/seismicsoftware/reference/authorization-code-login\n\
  \    use: User-delegated access. Required for the MCP server, which accepts user access tokens only.\n  - grant: authorization_code + PKCE\n    docs: https://developer.seismic.com/seismicsoftware/reference/pkce-get-the-users-authorization-code\n    pkce: S256\n    use: Public clients.\n  - grant: refresh_token\n    docs: https://developer.seismic.com/seismicsoftware/reference/exchange-the-refresh-token-for-an-access-refresh-token\n  - grant: urn:ietf:params:oauth:grant-type:device_code\n  - grant: urn:ietf:params:oauth:grant-type:token-exchange\n  - grant: password\n    note: Advertised by the authorization server and documented for token acquisition; not recommended for new integrations.\n    docs: https://developer.seismic.com/seismicsoftware/reference/get-a-token-using-username-and-password\n  client_auth: [client_secret_basic, client_secret_post]\n  scopes: scopes/seismic-scopes.yml\n  scopes_documented: 39\n  scopes_advertised: 389\n- name: openIdConnect\n  type: openIdConnect\n \
  \ openIdConnectUrl: https://auth.seismic.com/.well-known/openid-configuration\n  claims: [sub, email, email_verified, name, family_name, given_name, preferred_username, profile, picture, locale, updated_at]\n  docs: https://developer.seismic.com/seismicsoftware/reference/get-open-id-configuration\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    How the token is presented on every call — Authorization: Bearer <access_token>. This is the\n    only scheme declared in the OpenAPI documents; it describes transport, not the OAuth model above.\n  sources: [openapi/seismic-content-api-openapi.yml, openapi/seismic-users-api-openapi.yml, and 15 further openapi/ documents]\nresource_servers:\n- resource: https://api.seismic.com/integration/v2\n  auth: bearer JWT from https://auth.seismic.com\n- resource: https://api.seismic.com/scim/v2\n  auth: bearer JWT; SCIM 2.0 surface\n- resource: https://mcp.seismic.com/v1\n  auth: bearer JWT (user access token),\
  \ scope seismic.mcp\n  metadata: https://mcp.seismic.com/.well-known/oauth-protected-resource/v1\n  rfc: RFC 9728\nauthorization_model:\n  note: >-\n    Scope is necessary but not sufficient. Seismic states plainly for the MCP surface that the\n    seismic.mcp scope \"does not grant permission to invoke tools. Tool invocation requires\n    additional permissions configured by your tenant administrator.\" The same split applies across\n    the platform: token scope gates the API, tenant entitlement gates the capability. An agent that\n    treats a 403 as a token problem will loop.\nexternal_auth:\n  docs: https://developer.seismic.com/seismicsoftware/docs/external-auth\n  detail: Seismic apps can additionally federate to an external authorization service for their own backends.\ngaps:\n- >-\n  The OpenAPI documents declare no oauth2 securityScheme and no scope requirements per operation, so\n  a client generated from the spec alone cannot know which scope any operation needs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/authentication/seismic-authentication.yml
summary_line: oauth2/openIdConnect/http · 3 schemes
tags:
- Sales Enablement
- Content Management
- Document Generation
- Sales Content
- Buyer Engagement
- Revenue Enablement
- Analytics
- Learning
- SCIM
- MCP
---
