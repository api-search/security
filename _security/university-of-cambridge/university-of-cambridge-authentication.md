---
api_key_in: []
api_specs:
- filename: university-of-cambridge-group-api-openapi.yml
  format: yaml
  label: University of Cambridge group API
  slug: university-of-cambridge-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-cambridge/refs/heads/main/openapi/university-of-cambridge-group-api-openapi.yml
- filename: university-of-cambridge-ibis-api-openapi.yml
  format: yaml
  label: University of Cambridge ibis API
  slug: university-of-cambridge-ibis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-cambridge/refs/heads/main/openapi/university-of-cambridge-ibis-api-openapi.yml
- filename: university-of-cambridge-institution-api-openapi.yml
  format: yaml
  label: University of Cambridge institution API
  slug: university-of-cambridge-institution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-cambridge/refs/heads/main/openapi/university-of-cambridge-institution-api-openapi.yml
- filename: university-of-cambridge-person-api-openapi.yml
  format: yaml
  label: University of Cambridge person API
  slug: university-of-cambridge-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-cambridge/refs/heads/main/openapi/university-of-cambridge-person-api-openapi.yml
auth_types:
- http
- oauth2
- openIdConnect
- saml
description: ''
kind: authentication
layout: security
method: probed
name: University Of Cambridge Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Cambridge secures its APIs with http, oauth2, openIdConnect, and saml across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Cambridge
provider_slug: university-of-cambridge
scheme_count: 3
schemes:
- method: derived
  name: basicAuth
  scheme: basic
  sources:
  - openapi/_original/university-of-cambridge-lookup.yaml
  - https://www.lookup.cam.ac.uk/openapi-3.0.yaml
  surface: university-of-cambridge:university-of-cambridge-person-api
  type: http
  verified:
    note: Anonymous request rejected — the declared scheme is actually enforced.
    status: 401
    url: https://www.lookup.cam.ac.uk/api/v1/
- code_challenge_methods:
  - S256
  documentation: https://docs.raven.cam.ac.uk/en/latest/creating-oauth2-client-credentials/
  endpoints:
    authorization: https://api.apps.cam.ac.uk/oauth2/v1/auth
    jwks: https://api.apps.cam.ac.uk/oauth2/v1/.well-known/jwks.json
    token: https://api.apps.cam.ac.uk/oauth2/v1/token
    userinfo: https://api.apps.cam.ac.uk/oauth2/v1/userinfo
  grant_types:
  - client_credentials
  - authorization_code
  id_token_signing_alg_values:
  - RS256
  issuer: https://api.apps.cam.ac.uk/oauth2/v1/
  method: probed
  name: cambridgeApiGatewayOidc
  note: The discovery document declares no scopes_supported, so no scopes/ artifact is emitted — a scope list would have to be invented and this pipeline does not invent. PKCE (S256) is advertised, which is the strongest single ergonomics signal on the estate.
  openIdConnectUrl: https://api.apps.cam.ac.uk/oauth2/v1/.well-known/openid-configuration
  response_modes:
  - query
  - fragment
  response_types:
  - code
  scopes_advertised: none
  surface: university-of-cambridge:gateway
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  type: openIdConnect
- entityID: https://shib.raven.cam.ac.uk/shibboleth
  federation: UK Access Management Federation (republished via eduGAIN)
  metadata: https://shib.raven.cam.ac.uk/shibboleth
  method: probed
  name: ravenShibbolethSaml
  note: Web SSO for people, not an API credential. Recorded because SAML/Shibboleth is a named standard in the Kin Score education regime and because federation metadata is the one machine-readable artifact an institution cannot outsource.
  protocols:
  - urn:oasis:names:tc:SAML:2.0:protocol
  - urn:oasis:names:tc:SAML:1.1:protocol
  - urn:mace:shibboleth:1.0
  scopes_authoritative:
  - cam.ac.uk
  - eresources.lib.cam.ac.uk
  surface: university-of-cambridge:shibboleth-idp
  type: saml
slug: university-of-cambridge-authentication
source_filename: university-of-cambridge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nx-operator: institution\nsource: >-\n  Upgraded on 2026-08-19 from a derived read of the Lookup contract to a probed read of the\n  University's live identity surfaces: https://www.lookup.cam.ac.uk/openapi-3.0.yaml (first-party\n  OpenAPI 3.0, HTTP 200), https://api.apps.cam.ac.uk/oauth2/v1/.well-known/openid-configuration\n  (HTTP 200 application/json) and https://shib.raven.cam.ac.uk/shibboleth (HTTP 200, SAML 2.0 IdP\n  metadata). The prior record's `source:` pointed at openapi/university-of-cambridge-lookup.yaml,\n  a path that no longer exists in this repo — the pristine copy now lives at\n  openapi/_original/university-of-cambridge-lookup.yaml.\nnote: >-\n  Cambridge runs three distinct authentication regimes side by side, all institution-operated, and\n  they do not share a story: HTTP Basic on the legacy Lookup/Ibis web service, OAuth 2.0 / OpenID\n  Connect on the UIS API Gateway, and SAML 2.0 / Shibboleth for federated web\
  \ SSO. Only the first\n  is described in a machine-readable API contract.\nsummary:\n  types:\n  - http\n  - oauth2\n  - openIdConnect\n  - saml\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  method: derived\n  surface: university-of-cambridge:university-of-cambridge-person-api\n  sources:\n  - openapi/_original/university-of-cambridge-lookup.yaml\n  - https://www.lookup.cam.ac.uk/openapi-3.0.yaml\n  verified:\n    url: https://www.lookup.cam.ac.uk/api/v1/\n    status: 401\n    note: Anonymous request rejected — the declared scheme is actually enforced.\n- name: cambridgeApiGatewayOidc\n  type: openIdConnect\n  method: probed\n  surface: university-of-cambridge:gateway\n  openIdConnectUrl: https://api.apps.cam.ac.uk/oauth2/v1/.well-known/openid-configuration\n  issuer: https://api.apps.cam.ac.uk/oauth2/v1/\n  endpoints:\n    authorization: https://api.apps.cam.ac.uk/oauth2/v1/auth\n    token: https://api.apps.cam.ac.uk/oauth2/v1/token\n    userinfo: https://api.apps.cam.ac.uk/oauth2/v1/userinfo\n\
  \    jwks: https://api.apps.cam.ac.uk/oauth2/v1/.well-known/jwks.json\n  grant_types:\n  - client_credentials\n  - authorization_code\n  response_types:\n  - code\n  response_modes:\n  - query\n  - fragment\n  id_token_signing_alg_values:\n  - RS256\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - client_secret_basic\n  code_challenge_methods:\n  - S256\n  scopes_advertised: none\n  note: >-\n    The discovery document declares no scopes_supported, so no scopes/ artifact is emitted — a\n    scope list would have to be invented and this pipeline does not invent. PKCE (S256) is\n    advertised, which is the strongest single ergonomics signal on the estate.\n  documentation: https://docs.raven.cam.ac.uk/en/latest/creating-oauth2-client-credentials/\n- name: ravenShibbolethSaml\n  type: saml\n  method: probed\n  surface: university-of-cambridge:shibboleth-idp\n  entityID: https://shib.raven.cam.ac.uk/shibboleth\n  metadata: https://shib.raven.cam.ac.uk/shibboleth\n  protocols:\n\
  \  - urn:oasis:names:tc:SAML:2.0:protocol\n  - urn:oasis:names:tc:SAML:1.1:protocol\n  - urn:mace:shibboleth:1.0\n  scopes_authoritative:\n  - cam.ac.uk\n  - eresources.lib.cam.ac.uk\n  federation: UK Access Management Federation (republished via eduGAIN)\n  note: >-\n    Web SSO for people, not an API credential. Recorded because SAML/Shibboleth is a named standard\n    in the Kin Score education regime and because federation metadata is the one machine-readable\n    artifact an institution cannot outsource.\nnot_found:\n- name: api_keys\n  note: >-\n    The developer portal documents \"Using API Keys\" as a consumption pattern, but no key-issuance\n    endpoint or key description is reachable anonymously; registration is behind portal login.\n- name: mtls\n  note: No mutual-TLS requirement documented on any institution-operated host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-cambridge/refs/heads/main/authentication/university-of-cambridge-authentication.yml
summary_line: http/oauth2/openIdConnect/saml · 3 schemes
tags:
- Education
- Higher Education
- University
- Research
- United Kingdom
- Russell Group
- Identity
- Identity Federation
- API Gateway
- Developer Portal
- Research Data
- Open Access
- Research Repository
- Library
- Digital Collections
---
