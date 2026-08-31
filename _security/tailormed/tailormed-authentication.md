---
api_key_in: []
auth_types: []
description: Authentication profile derived from the OpenID Connect discovery document and the OAuth 2.0 authorization server metadata that TailorMed serves at auth.tailormed.com, plus the OAuth client configuration shipped in the public TailorMed platform SPA bundle. TailorMed publishes no OpenAPI, so no securityScheme block could be read; everything below was observed on the wire.
kind: authentication
layout: security
method: probed
name: Tailormed Authentication
name_suffix: Authentication
oauth_flows: []
overview: TailorMed declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: TailorMed
provider_slug: tailormed
scheme_count: 2
schemes:
- evidence: HTTP 200, application/json, fetched 2026-08-29
  issuer: https://auth.tailormed.com
  name: openIdConnect
  openIdConnectUrl: https://auth.tailormed.com/.well-known/openid-configuration
  type: openIdConnect
- evidence: https://auth.tailormed.com/.well-known/oauth-authorization-server, HTTP 200
  flows:
    authorizationCode:
      authorizationUrl: https://auth.tailormed.com/oauth2/v1/authorize
      refreshUrl: https://auth.tailormed.com/oauth2/v1/token
      tokenUrl: https://auth.tailormed.com/oauth2/v1/token
    deviceCode:
      deviceAuthorizationUrl: https://auth.tailormed.com/oauth2/v1/device/authorize
  name: oauth2
  type: oauth2
slug: tailormed-authentication
source_filename: tailormed-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://auth.tailormed.com/.well-known/openid-configuration\ndocs: https://hub.tailormed.co/dta/api-documentation\nname: TailorMed authentication profile\ndescription: >-\n  Authentication profile derived from the OpenID Connect discovery document and the\n  OAuth 2.0 authorization server metadata that TailorMed serves at auth.tailormed.com,\n  plus the OAuth client configuration shipped in the public TailorMed platform SPA\n  bundle. TailorMed publishes no OpenAPI, so no securityScheme block could be read;\n  everything below was observed on the wire.\nnote: >-\n  auth.tailormed.com is an Okta org authorization server on a TailorMed-controlled\n  custom domain (CNAME -> tailormed-platform.customdomains.okta-dnssec.com). Its issuer\n  is \"https://auth.tailormed.com\". A second, tenant-scoped authorization server is\n  reachable at /oauth2/default and reports issuer\n  \"https://tailormed-platform.okta.com/oauth2/default\". The\
  \ data-exchange APIs\n  (Application Data API, Claims Data API, HL7/FHIR) are documented only behind the\n  login on hub.tailormed.co, so their credential model could not be read publicly.\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.tailormed.com/.well-known/openid-configuration\n  issuer: https://auth.tailormed.com\n  evidence: 'HTTP 200, application/json, fetched 2026-08-29'\n- name: oauth2\n  type: oauth2\n  flows:\n    authorizationCode:\n      authorizationUrl: https://auth.tailormed.com/oauth2/v1/authorize\n      tokenUrl: https://auth.tailormed.com/oauth2/v1/token\n      refreshUrl: https://auth.tailormed.com/oauth2/v1/token\n    deviceCode:\n      deviceAuthorizationUrl: https://auth.tailormed.com/oauth2/v1/device/authorize\n  evidence: >-\n    https://auth.tailormed.com/.well-known/oauth-authorization-server, HTTP 200\nendpoints:\n  authorization: https://auth.tailormed.com/oauth2/v1/authorize\n  token: https://auth.tailormed.com/oauth2/v1/token\n\
  \  userinfo: https://auth.tailormed.com/oauth2/v1/userinfo\n  jwks: https://auth.tailormed.com/oauth2/v1/keys\n  introspection: https://auth.tailormed.com/oauth2/v1/introspect\n  revocation: https://auth.tailormed.com/oauth2/v1/revoke\n  end_session: https://auth.tailormed.com/oauth2/v1/logout\n  device_authorization: https://auth.tailormed.com/oauth2/v1/device/authorize\n  dynamic_client_registration: https://auth.tailormed.com/oauth2/v1/clients\ngrant_types:\n- authorization_code\n- implicit\n- refresh_token\n- password\n- 'urn:ietf:params:oauth:grant-type:device_code'\nresponse_types:\n- code\n- id_token\n- code id_token\n- code token\n- id_token token\n- code id_token token\ntoken_endpoint_auth_methods:\n- client_secret_basic\n- client_secret_post\n- client_secret_jwt\n- private_key_jwt\n- none\npkce:\n  supported: true\n  code_challenge_methods:\n  - S256\nid_token_signing_alg_values:\n- RS256\nsubject_types:\n- public\nobservations:\n- >-\n  PKCE is advertised with S256 only (no\
  \ plain), and the public SPA client uses the\n  authorization-code + PKCE flow with token_endpoint_auth_method \"none\".\n- >-\n  The resource-owner password grant is still advertised on the org authorization\n  server. That is an Okta org-server default rather than a documented TailorMed\n  integration path, but it is what the metadata says.\n- >-\n  Dynamic client registration is advertised at /oauth2/v1/clients; it was not\n  exercised.\napi_keys:\n  documented: unknown\n  note: >-\n    The Implementation Hub's own backend rejects unauthenticated calls with\n    {\"error\":\"Missing or invalid Authorization header\"} (HTTP 401 on\n    https://hub.tailormed.co/api/v1/openapi.json and every other /api/* path probed),\n    which shows a bearer-style Authorization header is expected, but the scheme is not\n    described on any public page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tailormed/refs/heads/main/authentication/tailormed-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Healthcare
- Health IT
- Medication Access
- Medication Affordability
- Financial Navigation
- Patient Assistance
- Pharmacy
- Oncology
- Revenue Cycle
- HL7
- FHIR
- Life Sciences
---
