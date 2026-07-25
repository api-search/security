---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Onetick Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: OneTick (OneMarketData) secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: OneTick (OneMarketData)
provider_slug: onetick
scheme_count: 2
schemes:
- description: OneTick Cloud WebAPI requests are authenticated with an OAuth2 Bearer access token issued by the OneTick Keycloak OMD realm. Machine access uses the client-credentials grant; the cloud dashboard and self-serve registration use the authorization-code flow (client_id acf_onetick_cloud). Unauthenticated requests to https://rest.cloud.onetick.com/omdwebapi/* receive a 302 redirect into the Keycloak authorization endpoint.
  flows:
  - flow: clientCredentials
    tokenUrl: https://cloud-auth.parent.onetick.com/realms/OMD/protocol/openid-connect/token
  - authorizationUrl: https://cloud-auth.parent.onetick.com/realms/OMD/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://cloud-auth.parent.onetick.com/realms/OMD/protocol/openid-connect/token
  name: OneTickCloudOAuth2
  sources:
  - well-known/onetick-openid-configuration.json
  type: oauth2
- description: Full OIDC discovery is published for the OMD realm (issuer https://cloud-auth.parent.onetick.com/realms/OMD), including jwks_uri, introspection, revocation, device-authorization, and pushed-authorization-request endpoints.
  name: OneTickOpenIDConnect
  openIdConnectUrl: https://cloud-auth.parent.onetick.com/realms/OMD/.well-known/openid-configuration
  sources:
  - well-known/onetick-openid-configuration.json
  type: openIdConnect
slug: onetick-authentication
source_filename: onetick-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://cloud-auth.parent.onetick.com/realms/OMD/.well-known/openid-configuration\ndocs: https://blog.onetick.com/basic-setup-of-webapi-access-to-onetick-cloud\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\n  token_style: Bearer\nschemes:\n- name: OneTickCloudOAuth2\n  type: oauth2\n  description: OneTick Cloud WebAPI requests are authenticated with an OAuth2 Bearer\n    access token issued by the OneTick Keycloak OMD realm. Machine access uses the\n    client-credentials grant; the cloud dashboard and self-serve registration use\n    the authorization-code flow (client_id acf_onetick_cloud). Unauthenticated requests\n    to https://rest.cloud.onetick.com/omdwebapi/* receive a 302 redirect into the\n    Keycloak authorization endpoint.\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://cloud-auth.parent.onetick.com/realms/OMD/protocol/openid-connect/token\n\
  \  - flow: authorizationCode\n    authorizationUrl: https://cloud-auth.parent.onetick.com/realms/OMD/protocol/openid-connect/auth\n    tokenUrl: https://cloud-auth.parent.onetick.com/realms/OMD/protocol/openid-connect/token\n  sources:\n  - well-known/onetick-openid-configuration.json\n- name: OneTickOpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://cloud-auth.parent.onetick.com/realms/OMD/.well-known/openid-configuration\n  description: Full OIDC discovery is published for the OMD realm (issuer\n    https://cloud-auth.parent.onetick.com/realms/OMD), including jwks_uri,\n    introspection, revocation, device-authorization, and pushed-authorization-request\n    endpoints.\n  sources:\n  - well-known/onetick-openid-configuration.json\ndetails:\n  issuer: https://cloud-auth.parent.onetick.com/realms/OMD\n  token_endpoint: https://cloud-auth.parent.onetick.com/realms/OMD/protocol/openid-connect/token\n  jwks_uri: https://cloud-auth.parent.onetick.com/realms/OMD/protocol/openid-connect/certs\n\
  \  token_endpoint_auth_methods:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - implicit\n  - password\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:uma-ticket\n  - urn:openid:params:grant-type:ciba\n  pkce_code_challenge_methods:\n  - plain\n  - S256\n  tls_client_certificate_bound_access_tokens: true\n  python_client: onetick-py in WebAPI mode reuses the same OAuth2 client credentials\n    (OTP_HTTP_ADDRESS=https://rest.cloud.onetick.com) and caches the access token\n    between queries (added in onetick-py 1.199.0).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onetick/refs/heads/main/authentication/onetick-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Financial
- Market Data
- Tick Data
- Historical Data
- Trading
- Analytics
- Surveillance
- Time Series
- Equities
- Options
---
