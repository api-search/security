---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Sollis Health Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Sollis Health secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Sollis Health
provider_slug: sollis-health
scheme_count: 2
schemes:
- applies_to: sollis-health:member-portal-api
  claims_supported:
  - emails
  - extension_employee_id
  - given_name
  - extension_sf_contact_id
  - extension_sf_email
  - idp
  - name
  - extension_IsAdmin
  - family_name
  - newUser
  - oid
  - sub
  - tfp
  - isForgotPassword
  - iss
  - iat
  - exp
  - aud
  - acr
  - nonce
  - auth_time
  endpoints:
    authorization: https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/b2c_1_google/oauth2/v2.0/authorize
    end_session: https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/b2c_1_google/oauth2/v2.0/logout
    jwks: https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/b2c_1_google/discovery/v2.0/keys
    token: https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/b2c_1_google/oauth2/v2.0/token
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://sollishealthprod.b2clogin.com/ee4f4213-0eca-4a72-bdd3-65661452caac/v2.0/
  name: b2c-openid-connect
  observations:
  - Federated sign-in — the user flow name (B2C_1_Google) and the `idp` claim indicate a social/federated identity provider is offered alongside local accounts.
  - Custom extension claims carry a Salesforce contact id (extension_sf_contact_id, extension_sf_email) and an admin flag (extension_IsAdmin), consistent with the Salesforce integration referenced from the staff console bundle.
  - Only `openid` is advertised in scopes_supported; the resource scope is requested separately by the application (see scopes/sollis-health-scopes.yml).
  openIdConnectUrl: https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/B2C_1_Google/v2.0/.well-known/openid-configuration
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
  - https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/B2C_1_Google/v2.0/.well-known/openid-configuration
  - https://mp.sollishealth.com/static/js/main.bee280e8.js
  subject_types_supported:
  - pairwise
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  type: openIdConnect
  user_flow: B2C_1_Google
- applies_to: sollis-health:navigator-api
  description: The Navigator staff console ships the Microsoft Authentication Library (MSAL) and authenticates against Microsoft identity. The application's own authority and client id are not asserted here — the MSAL default authority strings present in the bundle are library boilerplate, not Sollis configuration, and were not treated as evidence.
  name: msal-microsoft-identity
  observed:
    unauthenticated_request:
      status: 401
      url: https://navigator-api.sollishealth.com/v1/regions
  sources:
  - https://navigator.sollishealth.com/static/js/main.c89e96c4.js
  type: oauth2
slug: sollis-health-authentication
source_filename: sollis-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/B2C_1_Google/v2.0/.well-known/openid-configuration\nnote: >-\n  Sollis Health publishes no OpenAPI, so this profile is not derived from\n  securitySchemes. It is read from the anonymously-served OpenID Connect discovery\n  document of the company's Microsoft Entra External ID (Azure AD B2C) tenant, plus the\n  MSAL configuration shipped in the public JavaScript bundles of the two first-party\n  applications. No credentials were used and no access control was defeated.\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode, implicit]\n  identity_provider: Microsoft Entra External ID (Azure AD B2C)\n  tenant: sollishealthprod.onmicrosoft.com\n  tenant_id: ee4f4213-0eca-4a72-bdd3-65661452caac\n  public_developer_auth: false\n  public_auth_docs: null\nschemes:\n- name: b2c-openid-connect\n  type: openIdConnect\n  applies_to: sollis-health:member-portal-api\n\
  \  issuer: https://sollishealthprod.b2clogin.com/ee4f4213-0eca-4a72-bdd3-65661452caac/v2.0/\n  openIdConnectUrl: https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/B2C_1_Google/v2.0/.well-known/openid-configuration\n  user_flow: B2C_1_Google\n  endpoints:\n    authorization: https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/b2c_1_google/oauth2/v2.0/authorize\n    token: https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/b2c_1_google/oauth2/v2.0/token\n    end_session: https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/b2c_1_google/oauth2/v2.0/logout\n    jwks: https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/b2c_1_google/discovery/v2.0/keys\n  response_types_supported:\n  - code\n  - code id_token\n  - code token\n  - code id_token token\n  - id_token\n  - id_token token\n  - token\n  - token id_token\n  response_modes_supported: [query, fragment, form_post]\n  token_endpoint_auth_methods_supported:\
  \ [client_secret_post, client_secret_basic]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [pairwise]\n  scopes_supported: [openid]\n  claims_supported:\n  - emails\n  - extension_employee_id\n  - given_name\n  - extension_sf_contact_id\n  - extension_sf_email\n  - idp\n  - name\n  - extension_IsAdmin\n  - family_name\n  - newUser\n  - oid\n  - sub\n  - tfp\n  - isForgotPassword\n  - iss\n  - iat\n  - exp\n  - aud\n  - acr\n  - nonce\n  - auth_time\n  observations:\n  - Federated sign-in — the user flow name (B2C_1_Google) and the `idp` claim indicate\n    a social/federated identity provider is offered alongside local accounts.\n  - Custom extension claims carry a Salesforce contact id (extension_sf_contact_id,\n    extension_sf_email) and an admin flag (extension_IsAdmin), consistent with the\n    Salesforce integration referenced from the staff console bundle.\n  - Only `openid` is advertised in scopes_supported; the resource scope is requested\n    separately\
  \ by the application (see scopes/sollis-health-scopes.yml).\n  sources:\n  - https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/B2C_1_Google/v2.0/.well-known/openid-configuration\n  - https://mp.sollishealth.com/static/js/main.bee280e8.js\n- name: msal-microsoft-identity\n  type: oauth2\n  applies_to: sollis-health:navigator-api\n  description: >-\n    The Navigator staff console ships the Microsoft Authentication Library (MSAL) and\n    authenticates against Microsoft identity. The application's own authority and client\n    id are not asserted here — the MSAL default authority strings present in the bundle\n    are library boilerplate, not Sollis configuration, and were not treated as evidence.\n  observed:\n    unauthenticated_request:\n      url: https://navigator-api.sollishealth.com/v1/regions\n      status: 401\n  sources:\n  - https://navigator.sollishealth.com/static/js/main.c89e96c4.js\ndocs: null\ndocs_note: >-\n  Sollis Health publishes no developer authentication\
  \ documentation. There is no\n  developer portal, no API reference and no public sign-up for API credentials —\n  authentication exists only for members (Member Portal) and staff (Navigator).\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://sollishealthprod.b2clogin.com/sollishealthprod.onmicrosoft.com/B2C_1_Google/v2.0/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sollis-health/refs/heads/main/authentication/sollis-health-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Health
- Healthcare
- Concierge Medicine
- Urgent Care
- Emergency Care
- Membership
- Telehealth
- HIPAA
---
