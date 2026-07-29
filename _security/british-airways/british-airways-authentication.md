---
api_key_in:
- header
auth_types:
- openIdConnect
- apiKey
description: 'British Airways publishes no OpenAPI, so no securityScheme could be derived mechanically. This profile was assembled from the two authentication surfaces that are actually observable: the OpenID Connect discovery document of the Microsoft Entra External ID (CIAM) tenant that the NDC Communication Hub logs developers into, and the archived documentation for the client-key credential the NDC and legacy REST APIs consume. The hub login and the API credential are separate things — logging into ndc.ba.com does not grant API access; a client-key is issued disabled and only enabled through certification and a signed contract.'
kind: authentication
layout: security
method: searched
name: British Airways Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- deviceCode
overview: British Airways secures its APIs with openIdConnect and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, and deviceCode flow(s).
provider_name: British Airways
provider_slug: british-airways
scheme_count: 2
schemes:
- applies_to: Developer/partner login to the British Airways NDC Communication Hub (ndc.ba.com) — its documentation, sandbox screens and registration flows. Not the NDC message API itself.
  client_library: MSAL (bundled in the hub's Angular application)
  endpoints:
    authorization: https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/authorize
    device_authorization: https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/devicecode
    end_session: https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/logout
    jwks: https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/discovery/v2.0/keys
    mtls_token: https://mtlsauth.microsoft.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/token
    token: https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/token
    userinfo: https://graph.microsoft.com/oidc/userinfo
  frontchannel_logout_supported: true
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://45c0456f-2aef-40f6-847e-d3d957348527.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/v2.0
  name: EntraExternalID
  openIdConnectUrl: https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/v2.0/.well-known/openid-configuration
  provider: Microsoft Entra External ID (CIAM)
  response_modes_supported:
  - query
  - fragment
  - form_post
  response_types_supported:
  - code
  - id_token
  - code id_token
  - id_token token
  scopes:
  - openid
  - profile
  - email
  - offline_access
  scopes_artifact: scopes/british-airways-scopes.yml
  subject_types_supported:
  - pairwise
  tenant_id: 45c0456f-2aef-40f6-847e-d3d957348527
  tenant_region_scope: EU
  tls_client_certificate_bound_access_tokens: true
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - private_key_jwt
  - client_secret_basic
  - self_signed_tls_client_auth
  type: openIdConnect
- applies_to: The British Airways API credential. Documented for the retired public REST API ("Your unique key used to authorise access to the API") and carried forward as the credential issued at NDC registration ("Issue a new key for Shop and Order - test").
  in: header
  issuance: Issued on registration in a disabled state. Enabled for test only after the British Airways API and Services Trial Use Agreement is accepted, and for live only after B1 or B2 certification is passed and Live API Contracts are signed by both parties — live access follows within 5 working days of countersignature.
  name: client-key
  parameter_name: client-key
  source: https://web.archive.org/web/20211202/https://developer.iairgroup.com/british_airways/ApiInfo and https://web.archive.org/web/20210303183958/https://developer.iairgroup.com/british_airways/plans/ndc_certification
  status: The public REST API this key was documented against is decommissioned (api.ba.com returns ERR_596_SERVICE_NOT_FOUND). For NDC the credential model is described but no production host, header specification or token exchange is published.
  type: apiKey
slug: british-airways-authentication
source_filename: british-airways-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: >-\n  https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/v2.0/.well-known/openid-configuration\n  (fetched 2026-07-28, HTTP 200); https://ndc.ba.com/main.7a41cb6e4d2487f7.js (MSAL\n  configuration in the NDC hub application bundle); archived IAG Developer Programs portal\n  pages for the retired public REST API and the NDC certification flow.\ndescription: >-\n  British Airways publishes no OpenAPI, so no securityScheme could be derived mechanically.\n  This profile was assembled from the two authentication surfaces that are actually observable:\n  the OpenID Connect discovery document of the Microsoft Entra External ID (CIAM) tenant that\n  the NDC Communication Hub logs developers into, and the archived documentation for the\n  client-key credential the NDC and legacy REST APIs consume. The hub login and the API\n  credential are separate things — logging into ndc.ba.com does not grant API access; a\n\
  \  client-key is issued disabled and only enabled through certification and a signed contract.\nsummary:\n  types: [openIdConnect, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, implicit, deviceCode]\n  self_serve: false\n  gate: commercial-agreement\nschemes:\n  - name: EntraExternalID\n    type: openIdConnect\n    applies_to: >-\n      Developer/partner login to the British Airways NDC Communication Hub (ndc.ba.com) — its\n      documentation, sandbox screens and registration flows. Not the NDC message API itself.\n    openIdConnectUrl: https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/v2.0/.well-known/openid-configuration\n    issuer: https://45c0456f-2aef-40f6-847e-d3d957348527.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/v2.0\n    tenant_id: 45c0456f-2aef-40f6-847e-d3d957348527\n    tenant_region_scope: EU\n    provider: Microsoft Entra External ID (CIAM)\n    client_library: MSAL (bundled in the hub's Angular application)\n    endpoints:\n\
  \      authorization: https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/authorize\n      token: https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/token\n      device_authorization: https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/devicecode\n      end_session: https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/logout\n      jwks: https://baexternalid.ciamlogin.com/45c0456f-2aef-40f6-847e-d3d957348527/discovery/v2.0/keys\n      userinfo: https://graph.microsoft.com/oidc/userinfo\n      mtls_token: https://mtlsauth.microsoft.com/45c0456f-2aef-40f6-847e-d3d957348527/oauth2/v2.0/token\n    response_types_supported: [code, id_token, code id_token, id_token token]\n    response_modes_supported: [query, fragment, form_post]\n    token_endpoint_auth_methods_supported:\n      - client_secret_post\n      - private_key_jwt\n      - client_secret_basic\n      - self_signed_tls_client_auth\n\
  \    id_token_signing_alg_values_supported: [RS256]\n    subject_types_supported: [pairwise]\n    tls_client_certificate_bound_access_tokens: true\n    scopes: [openid, profile, email, offline_access]\n    scopes_artifact: scopes/british-airways-scopes.yml\n    frontchannel_logout_supported: true\n  - name: client-key\n    type: apiKey\n    in: header\n    parameter_name: client-key\n    applies_to: >-\n      The British Airways API credential. Documented for the retired public REST API\n      (\"Your unique key used to authorise access to the API\") and carried forward as the\n      credential issued at NDC registration (\"Issue a new key for Shop and Order - test\").\n    issuance: >-\n      Issued on registration in a disabled state. Enabled for test only after the British\n      Airways API and Services Trial Use Agreement is accepted, and for live only after B1 or\n      B2 certification is passed and Live API Contracts are signed by both parties — live\n      access follows within\
  \ 5 working days of countersignature.\n    source: >-\n      https://web.archive.org/web/20211202/https://developer.iairgroup.com/british_airways/ApiInfo\n      and https://web.archive.org/web/20210303183958/https://developer.iairgroup.com/british_airways/plans/ndc_certification\n    status: >-\n      The public REST API this key was documented against is decommissioned (api.ba.com returns\n      ERR_596_SERVICE_NOT_FOUND). For NDC the credential model is described but no production\n      host, header specification or token exchange is published.\nndc_api_authentication:\n  published: false\n  note: >-\n    British Airways publishes no authentication specification for the NDC message API itself.\n    No production base URL, no WSDL, no OpenAPI and no securityScheme are in the public domain.\n    What is documented is the process by which credentials are granted, not the wire format.\n    Anything more specific would be fabrication.\naccess_gate:\n  self_serve: false\n  value: commercial-agreement\n\
  \  steps:\n    - Register via https://ndc.ba.com/start/ndc-registrations and the NDC ServiceDesk\n    - Accept the British Airways API and Services Trial Use Agreement\n    - Receive a client-key, initially disabled\n    - Complete a B1 (direct) or B2 (via an NDC Service Provider) Certification Form\n    - Accept the Travel Agency Addendum if an IATA accredited agent\n    - Build and demonstrate successful test bookings against the test environment\n    - Sign Live API Contracts, tailored to business activity, countersigned by British Airways\n  docs:\n    - https://ndc.ba.com/start/ndc-registrations\n    - https://ndc.ba.com/start/build-and-test-the-api\n    - https://ndc.ba.com/start/get-certified-and-go-live\nrelated:\n  - scopes/british-airways-scopes.yml\n  - well-known/british-airways-well-known.yml\n  - conformance/british-airways-conformance.yml\n  - sandbox/british-airways-sandbox.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/british-airways/refs/heads/main/authentication/british-airways-authentication.yml
summary_line: openIdConnect/apiKey · 2 schemes
tags:
- Travel
- United Kingdom
- Aviation
- Airline
- Distribution
- NDC
- Booking
- Corporate Travel
- Airports
---
