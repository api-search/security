---
anonymous_access: true
api_key_in: []
api_specs:
- filename: ballerina-packages-api-openapi.yml
  format: yaml
  label: Ballerina Packages API
  slug: ballerina-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/openapi/ballerina-packages-api-openapi.yml
- filename: ballerina-connectors-api-openapi.yml
  format: yaml
  label: Ballerina Connectors API
  slug: ballerina-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/openapi/ballerina-connectors-api-openapi.yml
- filename: ballerina-triggers-api-openapi.yml
  format: yaml
  label: Ballerina Triggers API
  slug: ballerina-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/openapi/ballerina-triggers-api-openapi.yml
- filename: ballerina-docs-api-openapi.yml
  format: yaml
  label: Ballerina Docs API
  slug: ballerina-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/openapi/ballerina-docs-api-openapi.yml
auth_types: []
description: 'Ballerina Central runs a split authentication model, and the split is the important fact for an agent: every read operation on the public REST API is anonymous, and the only credentialed operation is publishing, which is not exposed over the documented REST surface at all — it is driven by the `bal` CLI. The OpenAPI in this repo therefore declares no securitySchemes, and that is correct rather than a gap.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ballerina Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ballerina declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Ballerina
provider_slug: ballerina
scheme_count: 2
schemes:
- applies_to: 'All probed read operations: GET /2.0/registry/packages, /2.0/registry/search-packages, /2.0/registry/packages/{org}/{name}, /2.0/registry/connectors, /2.0/registry/triggers and /2.0/docs/{org}/{name}/{version}.'
  evidence:
  - note: Returned a full package page with no Authorization header sent.
    status: 200
    url: https://api.central.ballerina.io/2.0/registry/packages?org=ballerina&limit=2&readme=false
  - note: Returned the full documentation model anonymously.
    status: 200
    url: https://api.central.ballerina.io/2.0/docs/ballerina/random/1.7.0
  id: anonymous
  type: none
  verified: probed
- account_required: true
  applies_to: Publishing and deprecating packages (`bal push`, `bal deprecate`).
  credential: Ballerina Central access token
  evidence:
  - status: 200
    url: https://ballerina.io/learn/publish-packages-to-ballerina-central/
  id: central-access-token
  obtained_from: https://central.ballerina.io/dashboard?tab=token
  rotation: Tokens are valid for one year from generation; the docs warn that an expired token surfaces as an unauthorized error on push.
  storage:
    environment_variable: BALLERINA_CENTRAL_ACCESS_TOKEN
    field: '[central] accesstoken'
    file: <USER_HOME>/.ballerina/Settings.toml
  type: bearer-token
  verified: searched
slug: ballerina-authentication
source_filename: ballerina-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://ballerina.io/learn/publish-packages-to-ballerina-central/\ndocs: https://ballerina.io/learn/publish-packages-to-ballerina-central/\nprovider: Ballerina\nproviderId: ballerina\ndescription: >-\n  Ballerina Central runs a split authentication model, and the split is the important fact for\n  an agent: every read operation on the public REST API is anonymous, and the only credentialed\n  operation is publishing, which is not exposed over the documented REST surface at all — it is\n  driven by the `bal` CLI. The OpenAPI in this repo therefore declares no securitySchemes, and\n  that is correct rather than a gap.\nschemes:\n  - id: anonymous\n    type: none\n    applies_to: >-\n      All probed read operations: GET /2.0/registry/packages, /2.0/registry/search-packages,\n      /2.0/registry/packages/{org}/{name}, /2.0/registry/connectors, /2.0/registry/triggers and\n      /2.0/docs/{org}/{name}/{version}.\n    verified: probed\n\
  \    evidence:\n      - url: https://api.central.ballerina.io/2.0/registry/packages?org=ballerina&limit=2&readme=false\n        status: 200\n        note: Returned a full package page with no Authorization header sent.\n      - url: https://api.central.ballerina.io/2.0/docs/ballerina/random/1.7.0\n        status: 200\n        note: Returned the full documentation model anonymously.\n  - id: central-access-token\n    type: bearer-token\n    applies_to: Publishing and deprecating packages (`bal push`, `bal deprecate`).\n    credential: Ballerina Central access token\n    obtained_from: https://central.ballerina.io/dashboard?tab=token\n    account_required: true\n    storage:\n      file: <USER_HOME>/.ballerina/Settings.toml\n      field: '[central] accesstoken'\n      environment_variable: BALLERINA_CENTRAL_ACCESS_TOKEN\n    rotation: >-\n      Tokens are valid for one year from generation; the docs warn that an expired token\n      surfaces as an unauthorized error on push.\n    verified:\
  \ searched\n    evidence:\n      - url: https://ballerina.io/learn/publish-packages-to-ballerina-central/\n        status: 200\noauth:\n  supported: false\n  note: >-\n    No OAuth 2.0 or OpenID Connect surface is published for the Central API — no scopes,\n    authorization server metadata or protected-resource metadata was found on any Ballerina\n    host (see well-known/ballerina-well-known.yml). Sign-in to central.ballerina.io itself is\n    an interactive web flow for humans, not a documented API authorization surface, so no\n    scopes/ artifact is written for this provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/authentication/ballerina-authentication.yml
summary_line: 2 schemes
tags:
- Integration
- Orchestrations
- Open-Source
- Programming Language
- Package Registry
- Developer Tools
- Code Generation
- Agent Skills
---
