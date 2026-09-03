---
api_key_in: []
api_specs:
- filename: massey-mro-dspace-openapi.yml
  format: yaml
  label: Massey Research Online OAI-PMH
  slug: mro-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/massey/refs/heads/main/openapi/massey-mro-dspace-openapi.yml
- filename: massey-mro-dspace-openapi.yml
  format: yaml
  label: Massey Research Online DSpace REST API
  slug: mro-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/massey/refs/heads/main/openapi/massey-mro-dspace-openapi.yml
- filename: massey-mapi-openapi.yml
  format: yaml
  label: Massey M-API WebService API v1
  slug: mapi-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/massey/refs/heads/main/openapi/massey-mapi-openapi.yml
auth_types: []
description: How each Massey University surface authenticates. Every entry carries the operator of the thing being authenticated against, because for a university most identity surfaces are either the institution's own federation endpoints or a vendor's login.
kind: authentication
layout: security
method: derived
name: Massey Authentication
name_suffix: Authentication
oauth_flows: []
overview: Massey University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Massey University
provider_slug: massey
scheme_count: 0
schemes: []
slug: massey-authentication
source_filename: massey-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Massey University\nproviderId: massey\ngenerated: '2026-09-01'\nmethod: derived\nacquisition: probed\nsource: live probes plus Massey University's own published M-API documentation\ndescription: >-\n  How each Massey University surface authenticates. Every entry carries the operator of the\n  thing being authenticated against, because for a university most identity surfaces are\n  either the institution's own federation endpoints or a vendor's login.\nsurfaces:\n  - id: massey:mapi-v1\n    name: M-API WebService API v1\n    operator: institution\n    scheme: apiKey\n    location: query\n    parameter: apikey\n    self_service: false\n    notes: >-\n      Massey's documentation states \"M-API V1 only work with a valid api key. You will need\n      to apply for one to use this api. Applications for new apikeys is not yet publicly\n      available.\" A demonstration key is printed on the docs page\
  \ for the page's own\n      examples and is described as returning cached, non-accurate data and not available for\n      production use. Failure is signalled in the body, not the HTTP status: a keyless\n      request returns HTTP 200 with `status: false` and `message: \"Invalid api key\"`.\n    evidence:\n      - url: https://www.massey.ac.nz/api/v1/\n        status: 200\n      - url: https://www.massey.ac.nz/api/v1/massey.cfc?method=get&path=news/articles&args=limit:2\n        status: 200\n  - id: massey:mro-rest\n    name: Massey Research Online DSpace REST API\n    operator: institution\n    scheme: mixed\n    self_service: false\n    notes: >-\n      Anonymous read is permitted on the repository root, communities and collections.\n      Item and bitstream listings require authentication - both returned HTTP 401\n      \"Authentication is required\" on 2026-09-01. DSpace 8 authenticates via\n      /server/api/authn (password, and typically Shibboleth on an institutional\n      deployment);\
  \ no public account registration surface was found.\n    evidence:\n      - url: https://mro.massey.ac.nz/server/api/core/communities\n        status: 200\n      - url: https://mro.massey.ac.nz/server/api/core/items\n        status: 401\n      - url: https://mro.massey.ac.nz/server/api/core/bitstreams\n        status: 401\n  - id: massey:mro-oai-pmh\n    name: Massey Research Online OAI-PMH\n    operator: institution\n    scheme: none\n    self_service: true\n    notes: Fully anonymous. No key, no registration, no quota published.\n    evidence:\n      - url: https://mro.massey.ac.nz/server/oai/request?verb=Identify\n        status: 200\n  - id: massey:idp-shibboleth\n    name: Massey University Shibboleth Identity Provider\n    operator: federation\n    scheme: saml2\n    entity_id: https://idp.massey.ac.nz/idp/shibboleth\n    scope: massey.ac.nz\n    federations: [Tuakiri Federation, eduGAIN]\n    self_service: false\n    notes: >-\n      The institution's own SAML 2.0 / Shibboleth IdP.\
  \ Service providers federate with it\n      through Tuakiri (the New Zealand Access Federation) and, internationally, eduGAIN. The\n      metadata document itself is public and machine-readable; the authentication it fronts\n      is for Massey affiliates only.\n    endpoints:\n      metadata: https://idp.massey.ac.nz/idp/shibboleth\n      sso_redirect: https://idp.massey.ac.nz/idp/profile/SAML2/Redirect/SSO\n      sso_post: https://idp.massey.ac.nz/idp/profile/SAML2/POST/SSO\n      slo_redirect: https://idp.massey.ac.nz/idp/profile/SAML2/Redirect/SLO\n    evidence:\n      - url: https://idp.massey.ac.nz/idp/shibboleth\n        status: 200\n  - id: massey:entra-id\n    name: Massey University Microsoft Entra ID tenant\n    operator: federation\n    scheme: oidc\n    tenant_id: 388728e1-bbd0-4378-98dc-f8682e644300\n    self_service: false\n    notes: >-\n      Massey operates a Microsoft Entra ID tenant discoverable by domain. The OpenID Connect\n      discovery document is public and machine-readable\
  \ and is the institution's own\n      identity surface; the accounts behind it are staff and student accounts. Region scope\n      \"OC\" (Oceania).\n    endpoints:\n      discovery: https://login.microsoftonline.com/massey.ac.nz/v2.0/.well-known/openid-configuration\n      issuer: https://login.microsoftonline.com/388728e1-bbd0-4378-98dc-f8682e644300/v2.0\n      authorization: https://login.microsoftonline.com/388728e1-bbd0-4378-98dc-f8682e644300/oauth2/v2.0/authorize\n      token: https://login.microsoftonline.com/388728e1-bbd0-4378-98dc-f8682e644300/oauth2/v2.0/token\n      jwks: https://login.microsoftonline.com/388728e1-bbd0-4378-98dc-f8682e644300/discovery/v2.0/keys\n    evidence:\n      - url: https://login.microsoftonline.com/massey.ac.nz/v2.0/.well-known/openid-configuration\n        status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/massey/refs/heads/main/authentication/massey-authentication.yml
summary_line: 0 schemes
tags:
- Education
- Higher Education
- University
- New Zealand
- Research
- Research Data
- Open Access
- Institutional Repository
- OAI-PMH
- DSpace
- Identity Federation
- Shibboleth
- SAML
- DataCite
- Crossref
- Library
---
