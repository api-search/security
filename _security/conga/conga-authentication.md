---
api_key_in: []
auth_types:
- oauth2
description: 'Conga''s REST API requires an OAuth 2.0 bearer token. Machine-to-machine access uses the client_credentials grant with a client_id/client_secret issued to an Integration User or an API-to-API connection. The token is obtained from a region-specific Conga login endpoint and passed as an Authorization: Bearer header on subsequent API calls. When using the API-to-API flow, callers also send a `user-id` header carrying the platform user ID so the API can apply the correct permissions.'
kind: authentication
layout: security
method: searched
name: Conga Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- implicit
overview: Conga secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, and implicit flow(s).
provider_name: Conga
provider_slug: conga
scheme_count: 2
schemes:
- extra_headers:
  - description: Platform user ID used to identify the caller and apply permissions.
    name: user-id
    required_for: API-to-API connection tokens
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  post_body:
  - grant_type
  - client_id
  - client_secret
  token_content_type: application/x-www-form-urlencoded
  token_endpoints:
  - region: NA
    url: https://login-rls.congacloud.com/api/v1/auth/connect/token
  - region: EU
    url: https://login.congacloud.eu/api/v1/auth/connect/token
  - region: AU
    url: https://login.congacloud.au/api/v1/auth/connect/token
  type: oauth2
- authorization_endpoint: https://login.conga.com/authorize
  device_authorization_endpoint: https://login.conga.com/oauth/device/code
  grant_types:
  - client_credentials
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  issuer: https://login.conga.com/
  name: DeveloperPortalOIDC
  openid_configuration: https://login.conga.com/.well-known/openid-configuration
  token_endpoint: https://login.conga.com/oauth/token
  type: openIdConnect
slug: conga-authentication
source_filename: conga-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.conga.com/platform/reference/authentication\ndocs: https://developer.conga.com/platform/reference/authentication\nsummary:\n  types: [oauth2]\n  primary: OAuth 2.0 bearer token\n  token_style: Authorization Bearer\n  oauth2_flows: [clientCredentials, authorizationCode, implicit]\n  identity_provider: >-\n    Conga login services (Auth0-backed for the developer portal / platform UI);\n    end users may federate through an external OAuth 2.0 identity provider.\ndescription: >-\n  Conga's REST API requires an OAuth 2.0 bearer token. Machine-to-machine access\n  uses the client_credentials grant with a client_id/client_secret issued to an\n  Integration User or an API-to-API connection. The token is obtained from a\n  region-specific Conga login endpoint and passed as an Authorization: Bearer\n  header on subsequent API calls. When using the API-to-API flow, callers also\n  send a `user-id` header carrying the\
  \ platform user ID so the API can apply the\n  correct permissions.\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  grant_type: client_credentials\n  token_content_type: application/x-www-form-urlencoded\n  token_endpoints:\n  - region: NA\n    url: https://login-rls.congacloud.com/api/v1/auth/connect/token\n  - region: EU\n    url: https://login.congacloud.eu/api/v1/auth/connect/token\n  - region: AU\n    url: https://login.congacloud.au/api/v1/auth/connect/token\n  post_body: [grant_type, client_id, client_secret]\n  extra_headers:\n  - name: user-id\n    required_for: API-to-API connection tokens\n    description: Platform user ID used to identify the caller and apply permissions.\n- name: DeveloperPortalOIDC\n  type: openIdConnect\n  openid_configuration: https://login.conga.com/.well-known/openid-configuration\n  issuer: https://login.conga.com/\n  authorization_endpoint: https://login.conga.com/authorize\n  token_endpoint: https://login.conga.com/oauth/token\n\
  \  device_authorization_endpoint: https://login.conga.com/oauth/device/code\n  grant_types:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\nprerequisites:\n- Create an Integration User and generate a client ID and client secret (Conga\n  Advantage Platform administration).\n- Or generate an API-to-API connection client ID/secret via Conga API Connections.\nreferences:\n- https://documentation.conga.com/en/advantage-platform-administration/current/conga-advantage-platform-for-administrators/managing-users/adding-users\n- https://documentation.conga.com/en/advantage-platform-administration/current/conga-advantage-platform-for-administrators/managing-organization/conga-api-connections\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conga/refs/heads/main/authentication/conga-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Enterprise Software
- Contract Lifecycle Management
- CPQ
- Revenue Lifecycle Management
- Document Automation
- E-Signature
- Contract Intelligence
- CRM
---
