---
api_key_in: []
auth_types: []
description: Authentication profile for Diligent Pharma. Diligent Pharma publishes no public developer API and no API authentication documentation, so this profile is derived entirely from the OpenID Connect / OAuth 2.0 discovery documents that clerk.diligentpharma.com serves for the authenticated Diligent360 application at 360.diligentpharma.com. It describes how a user (or an OAuth client registered with Diligent Pharma) signs into the Diligent360 web application — it is NOT a published developer-facing API authentication scheme, and there is no public client registration, key issuance, or token documentation.
kind: authentication
layout: security
method: probed
name: Diligent Pharma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Diligent Pharma declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Diligent Pharma
provider_slug: diligent-pharma
scheme_count: 2
schemes:
- backchannel_logout_supported: false
  claims_supported:
  - aud
  - iss
  - email
  - email_verified
  - preferred_username
  - exp
  - iat
  - given_name
  - family_name
  - name
  - picture
  - sub
  frontchannel_logout_supported: false
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://clerk.diligentpharma.com
  jwks_uri: https://clerk.diligentpharma.com/.well-known/jwks.json
  name: openIdConnect
  openIdConnectUrl: https://clerk.diligentpharma.com/.well-known/openid-configuration
  source: well-known/diligent-pharma-openid-configuration.json
  subject_types_supported:
  - public
  type: openIdConnect
  userinfo_endpoint: https://clerk.diligentpharma.com/oauth/userinfo
- code_challenge_methods_supported:
  - S256
  flows:
    authorizationCode:
      authorizationUrl: https://clerk.diligentpharma.com/oauth/authorize
      refreshUrl: https://clerk.diligentpharma.com/oauth/token
      scopes:
        email: Email address and verification state
        offline_access: Refresh token for long-lived access
        openid: OpenID Connect sign-in; issues an ID token
        private_metadata: Read the user's private metadata
        profile: Basic profile claims (name, given_name, family_name, picture, preferred_username)
        public_metadata: Read the user's public metadata
      tokenUrl: https://clerk.diligentpharma.com/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  introspection_endpoint: https://clerk.diligentpharma.com/oauth/token_info
  name: oauth2
  pkce_required_for_public_clients: true
  response_modes_supported:
  - form_post
  - query
  response_types_supported:
  - code
  revocation_endpoint: https://clerk.diligentpharma.com/oauth/token/revoke
  source: well-known/diligent-pharma-oauth-authorization-server.json
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
slug: diligent-pharma-authentication
source_filename: diligent-pharma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://clerk.diligentpharma.com/.well-known/openid-configuration\ndescription: >-\n  Authentication profile for Diligent Pharma. Diligent Pharma publishes no public\n  developer API and no API authentication documentation, so this profile is derived\n  entirely from the OpenID Connect / OAuth 2.0 discovery documents that\n  clerk.diligentpharma.com serves for the authenticated Diligent360 application at\n  360.diligentpharma.com. It describes how a user (or an OAuth client registered with\n  Diligent Pharma) signs into the Diligent360 web application — it is NOT a published\n  developer-facing API authentication scheme, and there is no public client\n  registration, key issuance, or token documentation.\nscope_of_this_profile: application-login\npublic_api_auth_documented: false\nidentity_provider:\n  vendor: Clerk\n  issuer: https://clerk.diligentpharma.com\n  host_ownership: >-\n    clerk.diligentpharma.com is a Diligent Pharma-controlled\
  \ hostname (Clerk custom\n    domain), so the discovery document is served from the provider's own domain.\n  discovered_via: >-\n    Diligent360 application JavaScript bundle\n    (https://360.diligentpharma.com/static/js/main.c2911d32.js), which references\n    https://clerk.diligentpharma.com/oauth/authorize\nschemes:\n  - name: openIdConnect\n    type: openIdConnect\n    openIdConnectUrl: https://clerk.diligentpharma.com/.well-known/openid-configuration\n    issuer: https://clerk.diligentpharma.com\n    userinfo_endpoint: https://clerk.diligentpharma.com/oauth/userinfo\n    jwks_uri: https://clerk.diligentpharma.com/.well-known/jwks.json\n    id_token_signing_alg_values_supported:\n      - RS256\n    subject_types_supported:\n      - public\n    claims_supported:\n      - aud\n      - iss\n      - email\n      - email_verified\n      - preferred_username\n      - exp\n      - iat\n      - given_name\n      - family_name\n      - name\n      - picture\n      - sub\n    backchannel_logout_supported:\
  \ false\n    frontchannel_logout_supported: false\n    source: well-known/diligent-pharma-openid-configuration.json\n  - name: oauth2\n    type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://clerk.diligentpharma.com/oauth/authorize\n        tokenUrl: https://clerk.diligentpharma.com/oauth/token\n        refreshUrl: https://clerk.diligentpharma.com/oauth/token\n        scopes:\n          openid: OpenID Connect sign-in; issues an ID token\n          profile: Basic profile claims (name, given_name, family_name, picture, preferred_username)\n          email: Email address and verification state\n          offline_access: Refresh token for long-lived access\n          public_metadata: Read the user's public metadata\n          private_metadata: Read the user's private metadata\n    grant_types_supported:\n      - authorization_code\n      - refresh_token\n    response_types_supported:\n      - code\n    response_modes_supported:\n      - form_post\n      -\
  \ query\n    token_endpoint_auth_methods_supported:\n      - client_secret_basic\n      - client_secret_post\n      - none\n    code_challenge_methods_supported:\n      - S256\n    pkce_required_for_public_clients: true\n    revocation_endpoint: https://clerk.diligentpharma.com/oauth/token/revoke\n    introspection_endpoint: https://clerk.diligentpharma.com/oauth/token_info\n    source: well-known/diligent-pharma-oauth-authorization-server.json\nobservations:\n  - Authorization Code with PKCE (S256) is the only interactive flow advertised; there\n    is no client_credentials grant, so there is no machine-to-machine service-account\n    path exposed on this authorization server.\n  - No dynamic client registration endpoint is advertised, so an OAuth client must be\n    provisioned by Diligent Pharma out of band.\n  - No public developer portal, key management page, or authentication guide was found\n    on any Diligent Pharma host.\ngaps:\n  - No public API authentication documentation.\n\
  \  - No documented API key, bearer token, or mTLS scheme.\n  - No /.well-known/oauth-protected-resource on any host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diligent-pharma/refs/heads/main/authentication/diligent-pharma-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Clinical Trials
- Life Sciences
- Pharmaceuticals
- Biotechnology
- Vendor Management
- Risk Management
- Quality Management
- Compliance
- GxP
- Auditing
- Software-as-a-Service
---
