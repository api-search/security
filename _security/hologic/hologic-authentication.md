---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Hologic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hologic declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Hologic
provider_slug: hologic
scheme_count: 1
schemes:
- dpop_signing_alg_values_supported:
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  - EdDSA
  dynamic_client_registration:
    endpoint: https://support.hologic.com/services/oauth2/register
    note: Advertised in the discovery document (RFC 7591). Not exercised by this pass — the pipeline does not register clients against a provider's identity server.
    supported: true
  endpoints:
    authorization: https://support.hologic.com/services/oauth2/authorize
    end_session: https://support.hologic.com/services/auth/idp/oidc/logout
    introspection: https://support.hologic.com/services/oauth2/introspect
    jwks_uri: https://support.hologic.com/id/keys
    registration: https://support.hologic.com/services/oauth2/register
    revocation: https://support.hologic.com/services/oauth2/revoke
    token: https://support.hologic.com/services/oauth2/token
    userinfo: https://support.hologic.com/services/oauth2/userinfo
  frontchannel_logout_supported: true
  grant_types_supported:
  - authorization_code
  - refresh_token
  id: hologic-support-oidc
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://support.hologic.com
  name: Hologic Support Community (OpenID Connect)
  openid_configuration: https://support.hologic.com/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    supported: true
  platform: Salesforce Experience Cloud
  response_types_supported:
  - code
  - token
  - token id_token
  subject_types_supported:
  - public
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: openIdConnect
slug: hologic-authentication
source_filename: hologic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: https://support.hologic.com/.well-known/openid-configuration\ndocs: https://support.hologic.com/s/login/\nnote: >-\n  Hologic publishes no public developer API and no OpenAPI document, so there are no\n  securitySchemes to derive an auth profile from. The one machine-readable identity contract\n  the company serves anywhere is the OpenID Connect discovery document at\n  support.hologic.com, fetched anonymously and saved verbatim to\n  well-known/hologic-openid-configuration.json. It governs sign-in to Hologic's customer\n  support community, not an API product. The community runs on Salesforce Experience Cloud,\n  so the endpoints and the scopes_supported list are the Salesforce platform's, served under\n  Hologic's own domain and issuer — stated here plainly so nobody reads this as a\n  Hologic-authored API authorization model.\nscope_of_this_profile: >-\n  Customer support portal sign-in (support.hologic.com). NOT an API product\
  \ authorization\n  model. No developer credential, API key, or token issuance surface is published by Hologic.\nschemes:\n  - id: hologic-support-oidc\n    type: openIdConnect\n    name: Hologic Support Community (OpenID Connect)\n    issuer: https://support.hologic.com\n    openid_configuration: https://support.hologic.com/.well-known/openid-configuration\n    endpoints:\n      authorization: https://support.hologic.com/services/oauth2/authorize\n      token: https://support.hologic.com/services/oauth2/token\n      userinfo: https://support.hologic.com/services/oauth2/userinfo\n      revocation: https://support.hologic.com/services/oauth2/revoke\n      introspection: https://support.hologic.com/services/oauth2/introspect\n      registration: https://support.hologic.com/services/oauth2/register\n      end_session: https://support.hologic.com/services/auth/idp/oidc/logout\n      jwks_uri: https://support.hologic.com/id/keys\n    grant_types_supported:\n      - authorization_code\n     \
  \ - refresh_token\n    response_types_supported:\n      - code\n      - token\n      - token id_token\n    pkce:\n      supported: true\n      code_challenge_methods: [S256]\n    token_endpoint_auth_methods_supported:\n      - client_secret_post\n      - client_secret_basic\n      - private_key_jwt\n    id_token_signing_alg_values_supported: [RS256]\n    dpop_signing_alg_values_supported: [RS256, RS384, RS512, ES256, ES384, ES512, EdDSA]\n    subject_types_supported: [public]\n    dynamic_client_registration:\n      supported: true\n      endpoint: https://support.hologic.com/services/oauth2/register\n      note: >-\n        Advertised in the discovery document (RFC 7591). Not exercised by this pass — the\n        pipeline does not register clients against a provider's identity server.\n    frontchannel_logout_supported: true\n    platform: Salesforce Experience Cloud\ngaps:\n  - No public API authentication documentation of any kind.\n  - No API key, personal access token, or developer\
  \ credential issuance surface.\n  - >-\n    No /.well-known/oauth-authorization-server or /.well-known/oauth-protected-resource on any\n    Hologic host; support.hologic.com returns 401 for both.\n  - >-\n    Device-level integration (DICOM network services, HL7 feeds) authenticates per-site at\n    installation time and is described only in PDF conformance statements and service manuals.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hologic/refs/heads/main/authentication/hologic-authentication.yml
summary_line: 1 scheme
tags:
- Fortune 1000
- Healthcare
- Medical Devices
- Medical Imaging
- Diagnostics
- Women's Health
- DICOM
- Life Sciences
---
