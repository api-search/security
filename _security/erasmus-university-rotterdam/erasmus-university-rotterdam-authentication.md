---
api_key_in: []
api_specs:
- filename: erasmus-university-rotterdam-repub-oai-pmh-openapi.yml
  format: yaml
  label: RePub OAI-PMH Metadata Harvesting Interface
  slug: repub-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/erasmus-university-rotterdam/refs/heads/main/openapi/erasmus-university-rotterdam-repub-oai-pmh-openapi.yml
auth_types:
- none
- http_basic
- oauth2
- saml2
description: ''
kind: authentication
layout: security
method: probed
name: Erasmus University Rotterdam Authentication
name_suffix: Authentication
oauth_flows: []
overview: Erasmus University Rotterdam secures its APIs with none, http_basic, oauth2, and saml2 across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Erasmus University Rotterdam
provider_slug: erasmus-university-rotterdam
scheme_count: 5
schemes:
- applies_to:
  - https://repub.eur.nl/oai
  - https://pure.eur.nl/ws/oai
  evidence: 'Both OAI-PMH endpoints answer Identify, ListMetadataFormats, ListSets and ListIdentifiers with HTTP 200 and no credential of any kind. Open metadata harvesting is deliberate: EUR is an OpenAIRE member and both endpoints are configured for OpenAIRE harvesting.'
  name: None (open harvesting)
  type: none
  x-operator: institution (repub) / tenant (pure)
- applies_to:
  - https://api.eur.nl/
  evidence: 'GET https://api.eur.nl/ returns 401 with WWW-Authenticate: Basic realm="kong" and body {"message":"Unauthorized"}. Unmatched paths return {"message":"no Route matched with those values"}. This is a Kong API gateway operated by EUR (api.eur.nl -> api2.eur.nl -> 145.5.1.16, EUR''s own address space) with HSTS max-age 31536000, X-Frame-Options DENY, X-Content-Type-Options nosniff and Cache-control no-store. No route, no documentation and no contract are exposed to an unauthenticated caller; the realm name is the only public signal of what it is.'
  name: Kong gateway credential
  scheme: basic
  type: http
  x-operator: institution
- applies_to:
  - https://pure.eur.nl/ws/api/
  evidence: https://pure.eur.nl/ws/api redirects to /ws/api/documentation/index.html (canonical https://api.elsevierpure.com/ws/api/documentation/index.html); https://pure.eur.nl/ws/api/524/openapi.json returns 401 application/json. Pure Web Service keys are issued per-integration by the institution's Pure administrators; there is no self-serve signup.
  name: Elsevier Pure Web Service API key
  type: apiKey
  x-operator: tenant
- applies_to:
  - https://canvas.eur.nl/api/v1/
  - https://canvas.eur.nl/login/oauth2/
  evidence: https://canvas.eur.nl/.well-known/openid-configuration returns 200 declaring issuer https://canvas.eur.nl, the three endpoints above, RS256 id_token signing, response_types_supported [code], grant_types_supported [authorization_code] and token_endpoint_auth_methods_supported [client_secret_basic, client_secret_post]. https://canvas.eur.nl/api/v1/courses returns 401 {"status":"unauthenticated",...}.
  flows:
  - authorizationUrl: https://canvas.eur.nl/login/oauth2/auth
    flow: authorizationCode
    jwksUri: https://canvas.eur.nl/login/oauth2/jwks
    scopes_supported:
    - openid
    tokenUrl: https://canvas.eur.nl/login/oauth2/token
  name: Canvas OAuth 2.0 / LTI 1.3 OIDC
  type: oauth2
  x-operator: tenant
- applies_to:
  - https://engine.surfconext.nl/authentication/idp/single-sign-on/
  evidence: EUR's identity provider is registered in the SURFconext federation as entityID https://sts.windows.net/715902d6-f63e-4b8d-929b-4bb170bad492/ (Microsoft Entra ID), with persistent and transient NameIDFormat support and shibmd:Scope covering eur.nl, student.eur.nl and eight faculty domains. This is how a human reaches every gated EUR surface; it is not a machine credential and grants no programmatic access.
  name: SURFconext SAML 2.0 federated sign-in
  type: saml2
  x-operator: tenant
slug: erasmus-university-rotterdam-authentication
source_filename: erasmus-university-rotterdam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource:\n- https://repub.eur.nl/oai?verb=Identify\n- https://api.eur.nl/\n- https://pure.eur.nl/ws/api/524/openapi.json\n- https://canvas.eur.nl/api/v1/courses\n- https://canvas.eur.nl/.well-known/openid-configuration\n- https://metadata.surfconext.nl/idps-metadata.xml\nnote: >-\n  Rewritten 2026-08-30. The previous file at this path was derived from\n  openapi/_original/erasmus-university-rotterdam-figshare-data.yaml and described Figshare's\n  OAuth 2.0 authorization-code flow at figshare.com/account/applications/authorize — Figshare's\n  authentication, not Erasmus University Rotterdam's. It was removed with the rest of the\n  Figshare-derived set. What follows is probed from EUR's own and EUR-tenanted hosts.\nsummary:\n  types:\n  - none\n  - http_basic\n  - oauth2\n  - saml2\n  public_keyless_surfaces: 2\n  credentialed_surfaces: 3\nschemes:\n- name: None (open harvesting)\n  type: none\n  applies_to:\n  - https://repub.eur.nl/oai\n\
  \  - https://pure.eur.nl/ws/oai\n  x-operator: institution (repub) / tenant (pure)\n  evidence: >-\n    Both OAI-PMH endpoints answer Identify, ListMetadataFormats, ListSets and ListIdentifiers\n    with HTTP 200 and no credential of any kind. Open metadata harvesting is deliberate: EUR\n    is an OpenAIRE member and both endpoints are configured for OpenAIRE harvesting.\n- name: Kong gateway credential\n  type: http\n  scheme: basic\n  applies_to:\n  - https://api.eur.nl/\n  x-operator: institution\n  evidence: >-\n    GET https://api.eur.nl/ returns 401 with WWW-Authenticate: Basic realm=\"kong\" and body\n    {\"message\":\"Unauthorized\"}. Unmatched paths return {\"message\":\"no Route matched with those\n    values\"}. This is a Kong API gateway operated by EUR (api.eur.nl -> api2.eur.nl ->\n    145.5.1.16, EUR's own address space) with HSTS max-age 31536000, X-Frame-Options DENY,\n    X-Content-Type-Options nosniff and Cache-control no-store. No route, no documentation and\n    no\
  \ contract are exposed to an unauthenticated caller; the realm name is the only public\n    signal of what it is.\n- name: Elsevier Pure Web Service API key\n  type: apiKey\n  applies_to:\n  - https://pure.eur.nl/ws/api/\n  x-operator: tenant\n  evidence: >-\n    https://pure.eur.nl/ws/api redirects to /ws/api/documentation/index.html (canonical\n    https://api.elsevierpure.com/ws/api/documentation/index.html);\n    https://pure.eur.nl/ws/api/524/openapi.json returns 401 application/json. Pure Web Service\n    keys are issued per-integration by the institution's Pure administrators; there is no\n    self-serve signup.\n- name: Canvas OAuth 2.0 / LTI 1.3 OIDC\n  type: oauth2\n  applies_to:\n  - https://canvas.eur.nl/api/v1/\n  - https://canvas.eur.nl/login/oauth2/\n  x-operator: tenant\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://canvas.eur.nl/login/oauth2/auth\n    tokenUrl: https://canvas.eur.nl/login/oauth2/token\n    jwksUri: https://canvas.eur.nl/login/oauth2/jwks\n\
  \    scopes_supported:\n    - openid\n  evidence: >-\n    https://canvas.eur.nl/.well-known/openid-configuration returns 200 declaring issuer\n    https://canvas.eur.nl, the three endpoints above, RS256 id_token signing,\n    response_types_supported [code], grant_types_supported [authorization_code] and\n    token_endpoint_auth_methods_supported [client_secret_basic, client_secret_post].\n    https://canvas.eur.nl/api/v1/courses returns 401 {\"status\":\"unauthenticated\",...}.\n- name: SURFconext SAML 2.0 federated sign-in\n  type: saml2\n  applies_to:\n  - https://engine.surfconext.nl/authentication/idp/single-sign-on/\n  x-operator: tenant\n  evidence: >-\n    EUR's identity provider is registered in the SURFconext federation as entityID\n    https://sts.windows.net/715902d6-f63e-4b8d-929b-4bb170bad492/ (Microsoft Entra ID), with\n    persistent and transient NameIDFormat support and shibmd:Scope covering eur.nl,\n    student.eur.nl and eight faculty domains. This is how a human reaches\
  \ every gated EUR\n    surface; it is not a machine credential and grants no programmatic access.\nabsent:\n- what: Public API key issuance or self-serve developer signup\n  evidence: >-\n    No developer portal exists. developer.eur.nl and developers.eur.nl have no DNS record.\n    www.eur.nl/.well-known/api-catalog, /llms.txt and /openapi.json all return the site's\n    soft 404 (\"Pagina niet gevonden\", 146,268 bytes of HTML under an HTTP 404).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/erasmus-university-rotterdam/refs/heads/main/authentication/erasmus-university-rotterdam-authentication.yml
summary_line: none/http_basic/oauth2/saml2 · 5 schemes
tags:
- University
- Higher Education
- Education
- Netherlands
- Rotterdam
- Research
- Research Data
- Open Access
- Repository
- OAI-PMH
- Identity Federation
- Course Catalog
- Learning Management
---
