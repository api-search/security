---
api_key_in: []
api_specs:
- filename: university-of-auckland-course-catalog-v3-openapi.yml
  format: yaml
  label: University of Auckland Course Catalog Api V3
  slug: course-catalog-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-auckland/refs/heads/main/openapi/university-of-auckland-course-catalog-v3-openapi.yml
- filename: university-of-auckland-classes-v2-openapi.yml
  format: yaml
  label: University of Auckland Classes Api V2
  slug: classes-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-auckland/refs/heads/main/openapi/university-of-auckland-classes-v2-openapi.yml
auth_types:
- apiKey
- oauth2
description: Authentication for the University of Auckland's own API gateway (apis.auckland.ac.nz, Kong) and its developer portal (developer.auckland.ac.nz/prd). Derived from the two OpenAPI documents the University publishes in that portal plus the portal's own guides; the scheme names and flow are the University's, the consolidation is ours.
kind: authentication
layout: security
method: derived
name: University Of Auckland Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: University of Auckland secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: University of Auckland
provider_slug: university-of-auckland
scheme_count: 2
schemes:
- declared_in:
  - openapi/_original/university-of-auckland-classes-v2-openapi.json
  - openapi/_original/university-of-auckland-course-catalog-v3-openapi.json
  name: apikey
  note: Both published specifications declare components.securitySchemes.apikey with type apiKey but do NOT declare `name` or `in`, and neither document carries a root-level or operation-level `security` requirement. The scheme is therefore under-specified in the University's own contract; the location of the key is not machine-readable from it.
  type: apiKey
- flow: clientCredentials
  name: OAuth2 client credentials
  note: The portal publishes three guides — "Trying API from developer portal", "Creating application client" and "Calling API using Client Credential flow" — establishing an application-client registration path and a client-credentials token exchange. The token endpoint is not published on the unauthenticated portal surface, so it is NOT recorded here.
  source: https://developer.auckland.ac.nz/prd/guides
  type: oauth2
slug: university-of-auckland-authentication
source_filename: university-of-auckland-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\ngenerated: '2026-08-30'\nmethod: derived\nsource:\n  - openapi/_original/university-of-auckland-classes-v2-openapi.json\n  - openapi/_original/university-of-auckland-course-catalog-v3-openapi.json\n  - https://developer.auckland.ac.nz/prd/guides\n  - probed 2026-08-30 against https://apis.auckland.ac.nz/\nx-operator: institution\nprovider: University of Auckland\nproviderId: university-of-auckland\ndescription: >-\n  Authentication for the University of Auckland's own API gateway (apis.auckland.ac.nz, Kong)\n  and its developer portal (developer.auckland.ac.nz/prd). Derived from the two OpenAPI\n  documents the University publishes in that portal plus the portal's own guides; the scheme\n  names and flow are the University's, the consolidation is ours.\nsummary:\n  types:\n    - apiKey\n    - oauth2\n  oauth2_flows:\n    - clientCredentials\n  registration: self-registration at https://developer.auckland.ac.nz/prd (portal login is OIDC)\nschemes:\n  - name: apikey\n  \
  \  type: apiKey\n    declared_in:\n      - openapi/_original/university-of-auckland-classes-v2-openapi.json\n      - openapi/_original/university-of-auckland-course-catalog-v3-openapi.json\n    note: >-\n      Both published specifications declare components.securitySchemes.apikey with type apiKey\n      but do NOT declare `name` or `in`, and neither document carries a root-level or\n      operation-level `security` requirement. The scheme is therefore under-specified in the\n      University's own contract; the location of the key is not machine-readable from it.\n  - name: OAuth2 client credentials\n    type: oauth2\n    flow: clientCredentials\n    source: https://developer.auckland.ac.nz/prd/guides\n    note: >-\n      The portal publishes three guides — \"Trying API from developer portal\", \"Creating\n      application client\" and \"Calling API using Client Credential flow\" — establishing an\n      application-client registration path and a client-credentials token exchange. The\
  \ token\n      endpoint is not published on the unauthenticated portal surface, so it is NOT recorded here.\nprobes:\n  - url: https://apis.auckland.ac.nz/\n    status: 404\n    body: '{\"message\":\"no Route matched with those values\"}'\n    note: Kong gateway root; confirms the gateway, not a dead host.\n  - url: https://apis.auckland.ac.nz/courses/v3/terms\n    status: 401\n    body: '{\"message\":\"Unauthorized\"}'\n  - url: https://apis.auckland.ac.nz/classes/v2/classes\n    status: 401\n    body: '{\"message\":\"Unauthorized\"}'\n  - url: https://developer.auckland.ac.nz/prd/\n    status: 200\n    note: Kong Developer Portal, workspace \"prd\", portal auth type openid-connect.\ngaps:\n  - No published token endpoint or authorization server metadata.\n  - No published scope list; scopes are NOT recorded because none are declared.\n  - securitySchemes.apikey omits `name` and `in`.\n  - No operation- or root-level `security` requirement in either specification.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-auckland/refs/heads/main/authentication/university-of-auckland-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- University
- Higher Education
- Education
- New Zealand
- Public Research University
- Universitas 21
- Course Catalog
- Student Records
- Research Data
- Research Repository
- Identity Federation
- OAI-PMH
---
