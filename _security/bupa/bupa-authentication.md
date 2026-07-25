---
api_key_in:
- header
auth_types:
- oauth2
- openIdConnect
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Bupa Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Bupa secures its APIs with oauth2, openIdConnect, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Bupa
provider_slug: bupa
scheme_count: 3
schemes:
- applies_to: Bupa Chile API portal (apidoc.bupa.cl)
  authorization_endpoint: https://login.microsoftonline.com/6faad805-0755-4412-981c-e2d4e4021ee7/oauth2/v2.0/authorize
  client_id: 744efffa-f93d-4137-b874-cef142712fa6
  discovery_http_status: 200
  discovery_url: https://login.microsoftonline.com/6faad805-0755-4412-981c-e2d4e4021ee7/v2.0/.well-known/openid-configuration
  end_session_endpoint: https://login.microsoftonline.com/6faad805-0755-4412-981c-e2d4e4021ee7/oauth2/v2.0/logout
  evidence: The MSAL configuration is declared in the portal's shipped Angular bundles (main-D6DO74WN.js and chunks), which also declare baseUrl https://api.bupa.cl/portal/ms-controller. The tenant's v2.0 OIDC discovery document returns HTTP 200 and was saved verbatim.
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://login.microsoftonline.com/6faad805-0755-4412-981c-e2d4e4021ee7/v2.0
  jwks_uri: https://login.microsoftonline.com/6faad805-0755-4412-981c-e2d4e4021ee7/discovery/v2.0/keys
  name: Microsoft Entra ID (OpenID Connect / OAuth 2.0 authorization code)
  openid_configuration: well-known/bupa-cl-entra-openid-configuration.json
  redirect_uri: https://apidoc.bupa.cl/public/login
  response_types_supported:
  - code
  - id_token
  - code id_token
  - id_token token
  scope: This authenticates access to the Chile developer portal itself. It is not published as the security scheme of any individual Bupa API — no such scheme document is public.
  scopes_supported:
  - openid
  - profile
  - email
  - offline_access
  status: confirmed
  subject_types_supported:
  - pairwise
  tenant: 6faad805-0755-4412-981c-e2d4e4021ee7
  tenant_region_scope: SA
  token_endpoint: https://login.microsoftonline.com/6faad805-0755-4412-981c-e2d4e4021ee7/oauth2/v2.0/token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - private_key_jwt
  - client_secret_basic
  - self_signed_tls_client_auth
  type: openIdConnect
  userinfo_endpoint: https://graph.microsoft.com/oidc/userinfo
- applies_to: https://api.bupa.cl/portal/ms-controller
  evidence: The portal bundle stores an Entra id_token in localStorage under "user" and calls the controller with it; every anonymous request to https://api.bupa.cl/, /portal/ms-controller, /portal/ms-controller/apis, /openapi.json and /swagger.json returns HTTP 401.
  name: Bupa Chile portal backend session
  scheme: bearer
  status: confirmed
  type: http
- applies_to: Bupa Australia APIs (api.bupa.com.au)
  caveat: INFERRED FROM THE PLATFORM, NOT FROM A PUBLISHED REFERENCE. Bupa documents no header name, no key issuance flow and no token endpoint publicly. The parameter name above is the Azure APIM default and has not been confirmed against a Bupa document. Do not treat it as an authoritative Bupa claim.
  evidence: portal.api.bupa.com.au is an Azure API Management managed developer portal (config.json declares APIM service banzprodapim01, managementApiVersion 2022-04-01-preview) and its public copy reads "Start with simple registration and get the keys to manage, build and test." Subscription-key header auth is the Azure APIM default.
  in: header
  name: Azure API Management subscription key
  parameter_name: Ocp-Apim-Subscription-Key
  status: inferred
  type: apiKey
slug: bupa-authentication
source_filename: bupa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  Live probes of Bupa's market-unit developer surfaces (portal.api.bupa.com.au,\n  apidoc.bupa.cl) plus the Entra ID OIDC discovery document captured in\n  well-known/bupa-cl-entra-openid-configuration.json\ndocs: null\nderived_from_openapi: false\nnote: >-\n  Bupa publishes no OpenAPI or Swagger definition anywhere on its public web\n  estate, so this profile cannot be derived from securitySchemes. It is\n  assembled instead from the platforms Bupa's two live market-unit developer\n  surfaces actually run on and from the one identity document that is\n  anonymously readable. Bupa does not publish an authentication reference page\n  for API consumers; access to the real scheme documentation is released only\n  after contacting the Bupa Integration Fabric Team. Everything below is\n  evidenced; nothing is inferred beyond what the evidence field states.\npublic_documentation:\n  published: false\n  reason: >-\n    Neither\
  \ market unit publishes an authentication guide. The Bupa Australia\n    portal's entire public onboarding text is three steps that all route\n    through a human team, and the Bupa Chile portal renders nothing before\n    sign-in.\nsummary:\n  types: [oauth2, openIdConnect, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  identity_providers: [Microsoft Entra ID]\n  confirmed: 2\n  inferred: 1\nschemes:\n- name: Microsoft Entra ID (OpenID Connect / OAuth 2.0 authorization code)\n  type: openIdConnect\n  status: confirmed\n  applies_to: Bupa Chile API portal (apidoc.bupa.cl)\n  openid_configuration: well-known/bupa-cl-entra-openid-configuration.json\n  discovery_url: https://login.microsoftonline.com/6faad805-0755-4412-981c-e2d4e4021ee7/v2.0/.well-known/openid-configuration\n  discovery_http_status: 200\n  issuer: https://login.microsoftonline.com/6faad805-0755-4412-981c-e2d4e4021ee7/v2.0\n  authorization_endpoint: https://login.microsoftonline.com/6faad805-0755-4412-981c-e2d4e4021ee7/oauth2/v2.0/authorize\n\
  \  token_endpoint: https://login.microsoftonline.com/6faad805-0755-4412-981c-e2d4e4021ee7/oauth2/v2.0/token\n  end_session_endpoint: https://login.microsoftonline.com/6faad805-0755-4412-981c-e2d4e4021ee7/oauth2/v2.0/logout\n  userinfo_endpoint: https://graph.microsoft.com/oidc/userinfo\n  jwks_uri: https://login.microsoftonline.com/6faad805-0755-4412-981c-e2d4e4021ee7/discovery/v2.0/keys\n  tenant: 6faad805-0755-4412-981c-e2d4e4021ee7\n  tenant_region_scope: SA\n  client_id: 744efffa-f93d-4137-b874-cef142712fa6\n  redirect_uri: https://apidoc.bupa.cl/public/login\n  response_types_supported: [code, id_token, code id_token, id_token token]\n  scopes_supported: [openid, profile, email, offline_access]\n  subject_types_supported: [pairwise]\n  id_token_signing_alg_values_supported: [RS256]\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - private_key_jwt\n  - client_secret_basic\n  - self_signed_tls_client_auth\n  evidence: >-\n    The MSAL configuration is declared in\
  \ the portal's shipped Angular bundles\n    (main-D6DO74WN.js and chunks), which also declare baseUrl\n    https://api.bupa.cl/portal/ms-controller. The tenant's v2.0 OIDC discovery\n    document returns HTTP 200 and was saved verbatim.\n  scope: >-\n    This authenticates access to the Chile developer portal itself. It is not\n    published as the security scheme of any individual Bupa API — no such\n    scheme document is public.\n- name: Bupa Chile portal backend session\n  type: http\n  scheme: bearer\n  status: confirmed\n  applies_to: https://api.bupa.cl/portal/ms-controller\n  evidence: >-\n    The portal bundle stores an Entra id_token in localStorage under \"user\" and\n    calls the controller with it; every anonymous request to\n    https://api.bupa.cl/, /portal/ms-controller, /portal/ms-controller/apis,\n    /openapi.json and /swagger.json returns HTTP 401.\n- name: Azure API Management subscription key\n  type: apiKey\n  in: header\n  parameter_name: Ocp-Apim-Subscription-Key\n\
  \  status: inferred\n  applies_to: Bupa Australia APIs (api.bupa.com.au)\n  evidence: >-\n    portal.api.bupa.com.au is an Azure API Management managed developer portal\n    (config.json declares APIM service banzprodapim01, managementApiVersion\n    2022-04-01-preview) and its public copy reads \"Start with simple\n    registration and get the keys to manage, build and test.\" Subscription-key\n    header auth is the Azure APIM default.\n  caveat: >-\n    INFERRED FROM THE PLATFORM, NOT FROM A PUBLISHED REFERENCE. Bupa documents\n    no header name, no key issuance flow and no token endpoint publicly. The\n    parameter name above is the Azure APIM default and has not been confirmed\n    against a Bupa document. Do not treat it as an authoritative Bupa claim.\nrelated:\n  well_known: well-known/bupa-well-known.yml\n  conformance: conformance/bupa-conformance.yml\n  domain_security: security/bupa-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bupa/refs/heads/main/authentication/bupa-authentication.yml
summary_line: oauth2/openIdConnect/apiKey · 3 schemes
tags:
- Insurance
- United Kingdom
- Health Insurance
- Life and Health
- Carrier
- Healthcare
- Aged Care
- Claims
- Policy Administration
- Partner Gated
---
