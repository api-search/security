---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Vitality Uk Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- password
- deviceCode
- refreshToken
- jwtBearer
- saml2Bearer
overview: Vitality secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, password, deviceCode, refreshToken, jwtBearer, and saml2Bearer flow(s).
provider_name: Vitality
provider_slug: vitality-uk
scheme_count: 2
schemes:
- claims:
    note: memberID / entityID / partyID are Vitality's own identity claims and are the clearest public signal of how the carrier keys members and parties across policy administration.
    standard:
    - sub
    - name
    - given_name
    - family_name
    - middle_name
    - nickname
    - preferred_username
    - profile
    - picture
    - website
    - gender
    - birthdate
    - zoneinfo
    - locale
    - updated_at
    - email
    - email_verified
    - phone_number
    - phone_number_verified
    - address
    - formatted
    - street_address
    - locality
    - region
    - postal_code
    - country
    - acr
    - iss
    vitality_specific:
    - memberID
    - entityID
    - entityId
    - entity_id
    - partyID
    - partyId
    - source
    - registered
    - roles
    - groups
    - upn
    - username
  endpoints:
    authorization: https://apis.vitality.co.uk/oauth2/authorize
    check_session_iframe: https://apis.vitality.co.uk/oidc/checksession
    device_authorization: https://wso2-prd-idsrv.tvc.vitality.co.uk:9443/oauth2/device_authorize
    end_session: https://apis.vitality.co.uk/oidc/logout
    introspection: https://wso2-prd-idsrv.tvc.vitality.co.uk:9443/oauth2/introspect
    jwks: https://apis.vitality.co.uk/oauth2/jwks
    registration: https://apis.vitality.co.uk/api/identity/oauth2/dcr/v1.1/register
    revocation: https://wso2-prd-idsrv.tvc.vitality.co.uk:9443/oauth2/revoke
    token: https://apis.vitality.co.uk/oauth2/token
    userinfo: https://apis.vitality.co.uk/oauth2/userinfo
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - urn:ietf:params:oauth:grant-type:saml2-bearer
  - iwa:ntlm
  - spoofToken
  - account_switch
  id_token_signing_alg:
  - RS256
  issuer: https://apis.vitality.co.uk/oauth2/token
  name: WSO2 API Manager OAuth2
  pkce:
    code_challenge_methods:
    - S256
    - plain
    supported: true
  request_object_signing_alg:
  - RS256
  - RS384
  - RS512
  - PS256
  - none
  response_modes:
  - query
  - fragment
  - form_post
  response_types:
  - code
  - token
  - id_token
  - code id_token
  - code token
  - id_token token
  - code id_token token
  - device
  - none
  session_management:
    backchannel_logout_session_supported: true
    backchannel_logout_supported: true
    check_session_iframe: true
  source: https://apis.vitality.co.uk/oauth2/token/.well-known/openid-configuration
  subject_types:
  - public
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
  userinfo_signing_alg:
  - RS256
- bearer_format: JWT
  name: Bearer token (gateway)
  note: Access tokens issued by the token endpoint above are presented to the apis.vitality.co.uk gateway as HTTP bearer tokens. No published API operation could be exercised anonymously to confirm the header name beyond the standard Authorization header.
  scheme: bearer
  type: http
slug: vitality-uk-authentication
source_filename: vitality-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://apis.vitality.co.uk/oauth2/token/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Vitality publishes no OpenAPI, so this profile is not derived from a spec — it\n  is read verbatim from the live OpenID Connect discovery document served by the\n  WSO2 Identity Server behind the apis.vitality.co.uk gateway, corroborated by\n  live probes of the token, authorization, userinfo, revocation and JWKS\n  endpoints and by the OAuth configuration embedded in Vitality's own\n  first-party Workplace Connect adviser application.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - password\n  - deviceCode\n  - refreshToken\n  - jwtBearer\n  - saml2Bearer\n  self_serve_signup: false\n  audience: commercial partners and first-party applications only\nschemes:\n- name: WSO2 API Manager OAuth2\n  type: oauth2\n  issuer: https://apis.vitality.co.uk/oauth2/token\n\
  \  source: https://apis.vitality.co.uk/oauth2/token/.well-known/openid-configuration\n  endpoints:\n    authorization: https://apis.vitality.co.uk/oauth2/authorize\n    token: https://apis.vitality.co.uk/oauth2/token\n    userinfo: https://apis.vitality.co.uk/oauth2/userinfo\n    jwks: https://apis.vitality.co.uk/oauth2/jwks\n    introspection: https://wso2-prd-idsrv.tvc.vitality.co.uk:9443/oauth2/introspect\n    revocation: https://wso2-prd-idsrv.tvc.vitality.co.uk:9443/oauth2/revoke\n    device_authorization: https://wso2-prd-idsrv.tvc.vitality.co.uk:9443/oauth2/device_authorize\n    registration: https://apis.vitality.co.uk/api/identity/oauth2/dcr/v1.1/register\n    end_session: https://apis.vitality.co.uk/oidc/logout\n    check_session_iframe: https://apis.vitality.co.uk/oidc/checksession\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n\
  \  - urn:ietf:params:oauth:grant-type:saml2-bearer\n  - iwa:ntlm\n  - spoofToken\n  - account_switch\n  response_types:\n  - code\n  - token\n  - id_token\n  - code id_token\n  - code token\n  - id_token token\n  - code id_token token\n  - device\n  - none\n  response_modes: [query, fragment, form_post]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  pkce:\n    supported: true\n    code_challenge_methods: [S256, plain]\n  id_token_signing_alg: [RS256]\n  userinfo_signing_alg: [RS256]\n  request_object_signing_alg: [RS256, RS384, RS512, PS256, none]\n  subject_types: [public]\n  session_management:\n    backchannel_logout_supported: true\n    backchannel_logout_session_supported: true\n    check_session_iframe: true\n  claims:\n    standard: [sub, name, given_name, family_name, middle_name, nickname,\n      preferred_username, profile, picture, website, gender, birthdate, zoneinfo,\n      locale, updated_at, email, email_verified, phone_number,\n      phone_number_verified,\
  \ address, formatted, street_address, locality, region,\n      postal_code, country, acr, iss]\n    vitality_specific: [memberID, entityID, entityId, entity_id, partyID, partyId,\n      source, registered, roles, groups, upn, username]\n    note: memberID / entityID / partyID are Vitality's own identity claims and are\n      the clearest public signal of how the carrier keys members and parties\n      across policy administration.\n- name: Bearer token (gateway)\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  note: Access tokens issued by the token endpoint above are presented to the\n    apis.vitality.co.uk gateway as HTTP bearer tokens. No published API operation\n    could be exercised anonymously to confirm the header name beyond the standard\n    Authorization header.\nverified:\n- probe: POST https://apis.vitality.co.uk/token (grant_type=client_credentials)\n  status: 401\n  body: '{\"error_description\":\"Unsupported Client Authentication Method!\",\"error\":\"invalid_client\"\
  }'\n  meaning: live token endpoint; rejects anonymous callers, requires partner-issued\n    client credentials\n- probe: GET https://apis.vitality.co.uk/authorize\n  status: 302\n  meaning: live authorization endpoint; redirects to the WSO2 authentication\n    endpoint OAuth error page for an invalid request\n- probe: GET https://apis.vitality.co.uk/oauth2/userinfo\n  status: 400\n  body: '{\"error_description\":\"Authorization or Content-Type header is missing\",\"error\":\"invalid_request\"}'\n- probe: GET https://apis.vitality.co.uk/oauth2/jwks\n  status: 200\n  meaning: 1 RSA RS256 signing key published\n- probe: GET https://apis.vitality.co.uk/oauth2/introspect\n  status: 401\n  body: '{\"code\":401,\"description\":\"AuthenticationHandler not found.\",\"message\":\"Unauthorized\"}'\n- probe: POST https://apis.vitality.co.uk/api/identity/oauth2/dcr/v1.1/register\n  status: 404\n  meaning: the dynamic client registration endpoint advertised in discovery is NOT\n    exposed through the\
  \ public gateway — client registration is a commercial\n    onboarding process, not self-serve\nonboarding:\n  self_serve: false\n  process: Client credentials are issued through Vitality's commercial partner\n    onboarding process. There is no developer signup form, no API key console and\n    no public dynamic client registration.\n  evidence: https://fintech.global/2025/08/20/vitality-accelerates-digital-transformation-with-wso2-api-gateway/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vitality-uk/refs/heads/main/authentication/vitality-uk-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Insurance
- United Kingdom
- Health Insurance
- Life Insurance
- Employee Benefits
- Carrier
- Policy Administration
- Underwriting
- Partner Gated
---
