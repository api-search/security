---
api_key_in: []
api_specs:
- filename: university-of-basel-admin-api-api-openapi.yml
  format: yaml
  label: DaSCH DSP-API — Admin API
  slug: university-of-basel-admin-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-basel/refs/heads/main/openapi/university-of-basel-admin-api-api-openapi.yml
- filename: university-of-basel-api-v2-api-openapi.yml
  format: yaml
  label: DaSCH DSP-API — API v2
  slug: university-of-basel-api-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-basel/refs/heads/main/openapi/university-of-basel-api-v2-api-openapi.yml
- filename: university-of-basel-api-v3-api-openapi.yml
  format: yaml
  label: DaSCH DSP-API — API v3
  slug: university-of-basel-api-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-basel/refs/heads/main/openapi/university-of-basel-api-v3-api-openapi.yml
- filename: university-of-basel-management-api-api-openapi.yml
  format: yaml
  label: DaSCH DSP-API — Management API
  slug: university-of-basel-management-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-basel/refs/heads/main/openapi/university-of-basel-management-api-api-openapi.yml
- filename: university-of-basel-ontology-mappings-api-openapi.yml
  format: yaml
  label: DaSCH DSP-API — Ontology Mappings
  slug: university-of-basel-ontology-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-basel/refs/heads/main/openapi/university-of-basel-ontology-mappings-api-openapi.yml
- filename: university-of-basel-experimental-api-openapi.yml
  format: yaml
  label: University of Basel Experimental API
  slug: university-of-basel-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-basel/refs/heads/main/openapi/university-of-basel-experimental-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: University Of Basel Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Basel secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Basel
provider_slug: university-of-basel
scheme_count: 2
schemes:
- bearer_format: JWT
  description: 'The supported authentication method. A client POSTs credentials to /v2/authentication and receives a JSON Web Token, then sends it on every secured request as `Authorization: Bearer <token>`.'
  name: httpAuth
  obtain:
    method: POST
    path: /v2/authentication
    request: '{"identifier_type": "iri|email|username", "password": "<password>"}'
    response: '{"token": "eyJ0eXAiOiJ..."}'
  revoke:
    effect: Invalidates the access token server-side; a later request presenting the same token is rejected. A genuine logout, not just a client-side discard.
    method: DELETE
    path: /v2/authentication
  scheme: bearer
  sources:
  - https://docs.dasch.swiss/latest/DSP-API/03-endpoints/api-v2/authentication/
  - openapi/_original/university-of-basel-dsp-api.yaml
  status: current
  surface: university-of-basel:dsp-api
  type: http
  verify:
    method: GET
    path: /v2/authentication
- description: 'HTTP Basic is still declared as a securityScheme in the contract, but the documentation states plainly: "Any other method of authentication is deprecated." Treat bearer JWT as the only supported path.'
  name: httpAuth1
  scheme: basic
  sources:
  - openapi/_original/university-of-basel-dsp-api.yaml
  - https://docs.dasch.swiss/latest/DSP-API/03-endpoints/api-v2/authentication/
  status: deprecated
  surface: university-of-basel:dsp-api
  type: http
slug: university-of-basel-authentication
source_filename: university-of-basel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  https://docs.dasch.swiss/latest/DSP-API/03-endpoints/api-v2/authentication/ (HTTP 200) and\n  https://docs.dasch.swiss/latest/DSP-API/05-internals/design/principles/authentication/, read\n  against the securitySchemes of https://api.dasch.swiss/api/docs/docs.yaml (v37.8.0); plus live\n  probes of https://edoc.unibas.ch/server/api/authn/status.\nprovider: University of Basel\nproviderId: university-of-basel\ndocs: https://docs.dasch.swiss/latest/DSP-API/03-endpoints/api-v2/authentication/\nsummary:\n  types:\n  - http\n  oauth2: false\n  openid_connect: false\n  mtls: false\n  api_keys: false\n  anonymous_read: true\nschemes:\n- name: httpAuth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  surface: university-of-basel:dsp-api\n  status: current\n  description: >-\n    The supported authentication method. A client POSTs credentials to /v2/authentication and\n    receives a JSON Web Token, then sends it on every\
  \ secured request as\n    `Authorization: Bearer <token>`.\n  obtain:\n    method: POST\n    path: /v2/authentication\n    request: '{\"identifier_type\": \"iri|email|username\", \"password\": \"<password>\"}'\n    response: '{\"token\": \"eyJ0eXAiOiJ...\"}'\n  verify:\n    method: GET\n    path: /v2/authentication\n  revoke:\n    method: DELETE\n    path: /v2/authentication\n    effect: >-\n      Invalidates the access token server-side; a later request presenting the same token is\n      rejected. A genuine logout, not just a client-side discard.\n  sources:\n  - https://docs.dasch.swiss/latest/DSP-API/03-endpoints/api-v2/authentication/\n  - openapi/_original/university-of-basel-dsp-api.yaml\n- name: httpAuth1\n  type: http\n  scheme: basic\n  surface: university-of-basel:dsp-api\n  status: deprecated\n  description: >-\n    HTTP Basic is still declared as a securityScheme in the contract, but the documentation states\n    plainly: \"Any other method of authentication is deprecated.\"\
  \ Treat bearer JWT as the only\n    supported path.\n  sources:\n  - openapi/_original/university-of-basel-dsp-api.yaml\n  - https://docs.dasch.swiss/latest/DSP-API/03-endpoints/api-v2/authentication/\nanonymous:\n  supported: true\n  operations: 54\n  note: >-\n    54 GET operations in the DSP-API contract are marked \"Publicly accessible\" and need no\n    credential — including project listing, full-text search, Gravsearch, ontology reads, IIIF\n    manifests, TEI rendering, /health and /version. This is the single largest agent-reachable\n    surface in the estate.\nother_surfaces:\n- api: university-of-basel:edoc-rest\n  host: edoc.unibas.ch\n  scheme: password realm\n  evidence:\n    url: https://edoc.unibas.ch/server/api/authn/status\n    status: 200\n    header: 'www-authenticate: password realm=\"DSpace REST API\"'\n    body_fragment: '{\"authenticated\": false, \"authenticationMethod\": null, \"type\": \"status\"}'\n  note: >-\n    DSpace 7 short-lived JWT obtained from POST\
  \ /server/api/authn/login, with a\n    DSPACE-XSRF-TOKEN CSRF header. Reads of public items need no credential. Only `password` is\n    advertised on the public REST surface — no Shibboleth method is exposed there.\n- api: university-of-basel:edoc-oai\n  host: edoc.unibas.ch\n  scheme: none\n  note: OAI-PMH is anonymous by protocol.\n- api: university-of-basel:swisscovery-sru\n  host: swisscovery.slsp.ch\n  scheme: none\n  note: >-\n    The SRU explain and search operations for institution zone 41SLSP_UBS answer anonymously\n    (probed 200 on 2026-08-27).\nscopes:\n  published: false\n  note: >-\n    No OAuth scopes exist. Authorization is enforced by the DSP permissions system — administrative\n    permissions and default object access permissions bound to a group within a project — not by\n    token scope. See data-model/university-of-basel-data-model.yml.\nwell_known:\n  openid_configuration: false\n  oauth_authorization_server: false\n  note: Both paths return 404 on every host in\
  \ the estate. See well-known/.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-basel/refs/heads/main/authentication/university-of-basel-authentication.yml
summary_line: http · 2 schemes
tags:
- Education
- Higher Education
- University
- Switzerland
- Research Data
- Open Access
- Institutional Repository
- Library
- Digital Humanities
---
