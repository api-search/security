---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Bupa Australia Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- hybrid
overview: Bupa Australia secures its APIs with oauth2 and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, and hybrid flow(s).
provider_name: Bupa Australia
provider_slug: bupa-australia
scheme_count: 3
schemes:
- authorizationUrl: https://partnerlogin.bupa.com.au/52bddae3-95ef-41bb-8c87-5561dead0bad/b2c_1a_prod_01_signup_signin/oauth2/v2.0/authorize
  claims_supported:
  - name
  - given_name
  - family_name
  - email
  - sub
  - tid
  - mobile
  - iss
  - iat
  - exp
  - aud
  - acr
  - nonce
  - auth_time
  code_challenge_methods_supported: null
  endSessionUrl: https://partnerlogin.bupa.com.au/52bddae3-95ef-41bb-8c87-5561dead0bad/b2c_1a_prod_01_signup_signin/oauth2/v2.0/logout
  guards: Bupa Partner Portal (https://partner.bupa.com.au/)
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://partnerlogin.bupa.com.au/52bddae3-95ef-41bb-8c87-5561dead0bad/v2.0/
  jwksUrl: https://partnerlogin.bupa.com.au/52bddae3-95ef-41bb-8c87-5561dead0bad/b2c_1a_prod_01_signup_signin/discovery/v2.0/keys
  name: partner-portal-b2c
  openIdConnectUrl: https://partnerlogin.bupa.com.au/52bddae3-95ef-41bb-8c87-5561dead0bad/B2C_1A_PROD_01_SIGNUP_SIGNIN/v2.0/.well-known/openid-configuration
  platform: Azure AD B2C
  policy: B2C_1A_PROD_01_SIGNUP_SIGNIN
  response_modes_supported:
  - query
  - fragment
  - form_post
  response_types_supported:
  - code
  - code id_token
  - code token
  - code id_token token
  - id_token
  - id_token token
  - token
  - token id_token
  scopes_supported:
  - openid
  sources:
  - well-known/bupa-australia-partner-b2c-openid-configuration.json
  status: confirmed
  subject_types_supported:
  - pairwise
  tokenUrl: https://partnerlogin.bupa.com.au/52bddae3-95ef-41bb-8c87-5561dead0bad/b2c_1a_prod_01_signup_signin/oauth2/v2.0/token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  type: openIdConnect
- authorizationUrl: https://login.microsoftonline.com/fee9c112-179f-46e3-ab98-f8d58602cf19/oauth2/v2.0/authorize
  evidence: 'https://portal.api.bupa.com.au/signin ships a signin-aad widget configured

    with tenants ["fee9c112-179f-46e3-ab98-f8d58602cf19"] alongside a

    signin-aad-b2c widget labelled "Sign-in / Register" — one path for Bupa

    staff, one for external registrants.

    '
  guards: Sign-in to the Bupa developer portal (https://portal.api.bupa.com.au/signin)
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://login.microsoftonline.com/fee9c112-179f-46e3-ab98-f8d58602cf19/v2.0
  name: developer-portal-entra
  openIdConnectUrl: https://login.microsoftonline.com/fee9c112-179f-46e3-ab98-f8d58602cf19/v2.0/.well-known/openid-configuration
  platform: Microsoft Entra ID
  response_types_supported:
  - code
  - id_token
  - code id_token
  - id_token token
  scopes_supported:
  - openid
  - profile
  - email
  - offline_access
  sources:
  - well-known/bupa-australia-portal-entra-openid-configuration.json
  status: confirmed
  subject_types_supported:
  - pairwise
  tenant: fee9c112-179f-46e3-ab98-f8d58602cf19
  tenant_region_scope: OC
  tokenUrl: https://login.microsoftonline.com/fee9c112-179f-46e3-ab98-f8d58602cf19/oauth2/v2.0/token
  type: openIdConnect
- evidence: 'portal.api.bupa.com.au is an Azure APIM managed developer portal

    (config.json names service banzprodapim01) and its home page copy reads

    "Start with simple registration and get the keys to manage, build and

    test." Subscription keys (Ocp-Apim-Subscription-Key by APIM default) are

    the platform norm, but Bupa publishes no header name, no scope and no base

    URL, so nothing is asserted here beyond the platform fact.

    '
  guards: The Bupa API gateway (api.bupa.com.au), once a partner is onboarded.
  in: null
  name: apim-subscription-key
  note: Inferred from the platform, not from any published API reference.
  parameter_name: null
  platform: Azure API Management
  status: implied
  type: apiKey
slug: bupa-australia-authentication
source_filename: bupa-australia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: |\n  Live fetches on 2026-07-25 of the two anonymously readable OpenID Connect\n  discovery documents in the Bupa Australia estate, plus the developer portal\n  sign-in page and its config.json. No OpenAPI exists for this provider, so\n  nothing here is derived from a spec.\ndocs: https://portal.api.bupa.com.au/get-started\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, implicit, hybrid]\n  api_authentication_published: false\n  note: |\n    Every authentication mechanism Bupa Australia publishes guards a HUMAN\n    sign-in, not an API. The developer portal releases API specifications only\n    after contacting the Bupa Integration Fabric Team, so no API base URL, no\n    key header name and no token audience is documented to anonymous\n    developers. The schemes below are what can actually be read from the\n    public surface, and they are recorded as what they are.\nschemes:\n\
  - name: partner-portal-b2c\n  type: openIdConnect\n  status: confirmed\n  guards: Bupa Partner Portal (https://partner.bupa.com.au/)\n  platform: Azure AD B2C\n  openIdConnectUrl: https://partnerlogin.bupa.com.au/52bddae3-95ef-41bb-8c87-5561dead0bad/B2C_1A_PROD_01_SIGNUP_SIGNIN/v2.0/.well-known/openid-configuration\n  issuer: https://partnerlogin.bupa.com.au/52bddae3-95ef-41bb-8c87-5561dead0bad/v2.0/\n  authorizationUrl: https://partnerlogin.bupa.com.au/52bddae3-95ef-41bb-8c87-5561dead0bad/b2c_1a_prod_01_signup_signin/oauth2/v2.0/authorize\n  tokenUrl: https://partnerlogin.bupa.com.au/52bddae3-95ef-41bb-8c87-5561dead0bad/b2c_1a_prod_01_signup_signin/oauth2/v2.0/token\n  endSessionUrl: https://partnerlogin.bupa.com.au/52bddae3-95ef-41bb-8c87-5561dead0bad/b2c_1a_prod_01_signup_signin/oauth2/v2.0/logout\n  jwksUrl: https://partnerlogin.bupa.com.au/52bddae3-95ef-41bb-8c87-5561dead0bad/b2c_1a_prod_01_signup_signin/discovery/v2.0/keys\n  policy: B2C_1A_PROD_01_SIGNUP_SIGNIN\n  scopes_supported:\
  \ [openid]\n  response_types_supported: [code, code id_token, code token, code id_token token, id_token, id_token token, token, token id_token]\n  response_modes_supported: [query, fragment, form_post]\n  token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [pairwise]\n  claims_supported: [name, given_name, family_name, email, sub, tid, mobile, iss, iat, exp, aud, acr, nonce, auth_time]\n  code_challenge_methods_supported: null\n  sources: [well-known/bupa-australia-partner-b2c-openid-configuration.json]\n- name: developer-portal-entra\n  type: openIdConnect\n  status: confirmed\n  guards: Sign-in to the Bupa developer portal (https://portal.api.bupa.com.au/signin)\n  platform: Microsoft Entra ID\n  tenant: fee9c112-179f-46e3-ab98-f8d58602cf19\n  tenant_region_scope: OC\n  openIdConnectUrl: https://login.microsoftonline.com/fee9c112-179f-46e3-ab98-f8d58602cf19/v2.0/.well-known/openid-configuration\n\
  \  issuer: https://login.microsoftonline.com/fee9c112-179f-46e3-ab98-f8d58602cf19/v2.0\n  authorizationUrl: https://login.microsoftonline.com/fee9c112-179f-46e3-ab98-f8d58602cf19/oauth2/v2.0/authorize\n  tokenUrl: https://login.microsoftonline.com/fee9c112-179f-46e3-ab98-f8d58602cf19/oauth2/v2.0/token\n  scopes_supported: [openid, profile, email, offline_access]\n  response_types_supported: [code, id_token, code id_token, id_token token]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [pairwise]\n  sources: [well-known/bupa-australia-portal-entra-openid-configuration.json]\n  evidence: |\n    https://portal.api.bupa.com.au/signin ships a signin-aad widget configured\n    with tenants [\"fee9c112-179f-46e3-ab98-f8d58602cf19\"] alongside a\n    signin-aad-b2c widget labelled \"Sign-in / Register\" — one path for Bupa\n    staff, one for external registrants.\n- name: apim-subscription-key\n  type: apiKey\n  status: implied\n  guards: The Bupa API gateway (api.bupa.com.au),\
  \ once a partner is onboarded.\n  platform: Azure API Management\n  in: null\n  parameter_name: null\n  evidence: |\n    portal.api.bupa.com.au is an Azure APIM managed developer portal\n    (config.json names service banzprodapim01) and its home page copy reads\n    \"Start with simple registration and get the keys to manage, build and\n    test.\" Subscription keys (Ocp-Apim-Subscription-Key by APIM default) are\n    the platform norm, but Bupa publishes no header name, no scope and no base\n    URL, so nothing is asserted here beyond the platform fact.\n  note: Inferred from the platform, not from any published API reference.\nprobes:\n- url: https://api.bupa.com.au/.well-known/openid-configuration\n  status: 502\n- url: https://api.bupa.com.au/.well-known/oauth-authorization-server\n  status: 502\n- url: https://portal.api.bupa.com.au/.well-known/openid-configuration\n  status: 404\n- url: https://portal.api.bupa.com.au/.well-known/oauth-authorization-server\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bupa-australia/refs/heads/main/authentication/bupa-australia-authentication.yml
summary_line: oauth2/openIdConnect · 3 schemes
tags:
- Insurance
- Australia
- Health Insurance
- Private Health Insurance
- Carrier
- Healthcare
- Claims
- Policy Administration
- Employee Benefits
- Partner Gated
---
