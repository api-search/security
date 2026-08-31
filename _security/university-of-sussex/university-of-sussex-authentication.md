---
api_key_in: []
auth_types:
- saml2
- oidc
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: University Of Sussex Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- refreshToken
- deviceCode
- ciba
overview: University of Sussex secures its APIs with saml2, oidc, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, refreshToken, deviceCode, and ciba flow(s).
provider_name: University of Sussex
provider_slug: university-of-sussex
scheme_count: 3
schemes:
- entity_id: https://idp.sussex.ac.uk/shibboleth
  federation: UK Access Management Federation / eduGAIN (scope asserted in metadata; federation registration not independently confirmed on 2026-08-30)
  metadata_url: https://idp.sussex.ac.uk/idp/shibboleth
  name: Shibboleth SAML 2.0 Identity Provider
  scope: sussex.ac.uk
  sources:
  - status: 200
    url: https://idp.sussex.ac.uk/idp/shibboleth
  type: saml2
  x-operator: institution
- discovery_url: https://okta.sussex.ac.uk/.well-known/openid-configuration
  dpop_signing_alg_values_supported:
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  endpoints:
    device_authorization: https://okta.sussex.ac.uk/oauth2/v1/device/authorize
    dynamic_client_registration: https://okta.sussex.ac.uk/oauth2/v1/clients
    end_session: https://okta.sussex.ac.uk/oauth2/v1/logout
    introspection: https://okta.sussex.ac.uk/oauth2/v1/introspect
    jwks: https://okta.sussex.ac.uk/oauth2/v1/keys
    pushed_authorization_request: https://okta.sussex.ac.uk/oauth2/v1/par
    revocation: https://okta.sussex.ac.uk/oauth2/v1/revoke
    userinfo: https://okta.sussex.ac.uk/oauth2/v1/userinfo
  flows:
  - authorizationUrl: https://okta.sussex.ac.uk/oauth2/v1/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://okta.sussex.ac.uk/oauth2/v1/token
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://okta.sussex.ac.uk
  name: Okta OpenID Connect (Sussex tenant)
  sources:
  - status: 200
    url: https://okta.sussex.ac.uk/.well-known/openid-configuration
  type: oidc
  vendor_host: sussexac.customdomains.okta.com
  x-operator: tenant
- name: Canvas LMS (Sussex tenant)
  sources:
  - status: 401
    url: https://canvas.sussex.ac.uk/api/v1/accounts
  - status: 200
    url: https://canvas.sussex.ac.uk/api/lti/security/jwks
  summary: canvas.sussex.ac.uk answers /api/v1/* with 401 {"status":"unauthenticated"}. Canvas uses OAuth2 bearer tokens issued per user; there is no public client registration on this tenant.
  type: oauth2
  vendor_host: universityofsussex-vanity.instructure.com
  x-operator: tenant
slug: university-of-sussex-authentication
source_filename: university-of-sussex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "# x-method: derived\n# x-source-url: https://okta.sussex.ac.uk/.well-known/openid-configuration\n# Authorship: written by API Evangelist tooling from LIVE PROBES of the URL above.\n# `x-method: derived` is the provenance-manifest vocabulary (build-provenance-manifest.py,\n# which has no `probed` term); `method: probed` below is the enrichment-pipeline vocabulary.\n# They agree: this artifact is ours, and its facts came off the wire, not off a claim.\n# University of Sussex — authentication surfaces\n# Rebuilt 2026-08-30. The previous version of this file was DERIVED FROM FIGSHARE'S\n# generic v2 OpenAPI and described Figshare's OAuth server, not the university's.\n# It has been removed. Everything below was probed live against Sussex-controlled hosts.\ngenerated: '2026-08-30'\nmethod: probed\nsource: live HTTPS probes of idp.sussex.ac.uk and okta.sussex.ac.uk\nprovider: University of Sussex\nproviderId: university-of-sussex\n\nsummary:\n  types:\n  - saml2\n  - oidc\n  - oauth2\n\
  \  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - refreshToken\n  - deviceCode\n  - ciba\n  public_developer_registration: false\n  note: >-\n    Neither surface is a public developer API. Both gate access to enrolled Sussex\n    applications and require institutional affiliation; there is no self-serve client\n    registration for outside developers. They are recorded because they are the\n    institution's only live, machine-readable contracts.\n\nschemes:\n- name: Shibboleth SAML 2.0 Identity Provider\n  type: saml2\n  x-operator: institution\n  entity_id: https://idp.sussex.ac.uk/shibboleth\n  metadata_url: https://idp.sussex.ac.uk/idp/shibboleth\n  scope: sussex.ac.uk\n  federation: UK Access Management Federation / eduGAIN (scope asserted in metadata; federation\n    registration not independently confirmed on 2026-08-30)\n  sources:\n  - url: https://idp.sussex.ac.uk/idp/shibboleth\n    status: 200\n\n- name: Okta OpenID Connect (Sussex tenant)\n  type: oidc\n  x-operator:\
  \ tenant\n  issuer: https://okta.sussex.ac.uk\n  discovery_url: https://okta.sussex.ac.uk/.well-known/openid-configuration\n  vendor_host: sussexac.customdomains.okta.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://okta.sussex.ac.uk/oauth2/v1/authorize\n    tokenUrl: https://okta.sussex.ac.uk/oauth2/v1/token\n    pkce: S256\n  endpoints:\n    userinfo: https://okta.sussex.ac.uk/oauth2/v1/userinfo\n    jwks: https://okta.sussex.ac.uk/oauth2/v1/keys\n    introspection: https://okta.sussex.ac.uk/oauth2/v1/introspect\n    revocation: https://okta.sussex.ac.uk/oauth2/v1/revoke\n    end_session: https://okta.sussex.ac.uk/oauth2/v1/logout\n    device_authorization: https://okta.sussex.ac.uk/oauth2/v1/device/authorize\n    pushed_authorization_request: https://okta.sussex.ac.uk/oauth2/v1/par\n    dynamic_client_registration: https://okta.sussex.ac.uk/oauth2/v1/clients\n  id_token_signing_alg_values_supported:\n  - RS256\n  dpop_signing_alg_values_supported:\n  - RS256\n\
  \  - RS384\n  - RS512\n  - ES256\n  - ES384\n  - ES512\n  sources:\n  - url: https://okta.sussex.ac.uk/.well-known/openid-configuration\n    status: 200\n\n- name: Canvas LMS (Sussex tenant)\n  type: oauth2\n  x-operator: tenant\n  summary: >-\n    canvas.sussex.ac.uk answers /api/v1/* with 401 {\"status\":\"unauthenticated\"}. Canvas uses\n    OAuth2 bearer tokens issued per user; there is no public client registration on this tenant.\n  vendor_host: universityofsussex-vanity.instructure.com\n  sources:\n  - url: https://canvas.sussex.ac.uk/api/v1/accounts\n    status: 401\n  - url: https://canvas.sussex.ac.uk/api/lti/security/jwks\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-sussex/refs/heads/main/authentication/university-of-sussex-authentication.yml
summary_line: saml2/oidc/oauth2 · 3 schemes
tags:
- University
- Higher Education
- Education
- United Kingdom
- Russell Group
- Public Research University
- Identity Federation
- Research Repository
- Library
- Learning Management
- Research
- Open Access
---
