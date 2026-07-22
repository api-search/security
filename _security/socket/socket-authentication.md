---
api_key_in: []
api_specs:
- filename: socket-openapi-original.json
  format: json
  label: Socket API
  slug: socket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-openapi-original.json
auth_types:
- http
description: 'Socket authenticates REST API requests with an organization API token. The OpenAPI declares two HTTP schemes: bearer and basic. The same token is used either as an Authorization Bearer credential or as the Basic-auth username (with an empty password). Tokens carry fine-grained scopes (see scopes/socket-scopes.yml) and are metered by quota.'
kind: authentication
layout: security
method: searched
name: Socket Authentication
name_suffix: Authentication
oauth_flows: []
overview: Socket secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Socket
provider_slug: socket
scheme_count: 2
schemes:
- description: 'Authorization: Bearer <ORG_API_TOKEN>'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/socket-openapi-original.json
  type: http
- description: HTTP Basic with the API token as the username and an empty password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/socket-openapi-original.json
  type: http
slug: socket-authentication
source_filename: socket-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/socket-openapi-original.json\ndocs: https://docs.socket.dev/reference/authentication\ndescription: >-\n  Socket authenticates REST API requests with an organization API token. The OpenAPI declares\n  two HTTP schemes: bearer and basic. The same token is used either as an Authorization Bearer\n  credential or as the Basic-auth username (with an empty password). Tokens carry fine-grained\n  scopes (see scopes/socket-scopes.yml) and are metered by quota.\nsummary:\n  types: [http]\n  http_schemes: [bearer, basic]\n  api_key_in: []\n  oauth2_flows: []\n  token_scopes: true\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Authorization: Bearer <ORG_API_TOKEN>'\n  sources: [openapi/socket-openapi-original.json]\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic with the API token as the username and an empty password.\n  sources: [openapi/socket-openapi-original.json]\n\
  token_management:\n  docs: https://docs.socket.dev/reference/creating-and-managing-api-tokens\n  operations: [postAPIToken, getAPITokens, postAPITokenUpdate, postAPITokensRotate, postAPITokensRevoke]\n  scopes_artifact: scopes/socket-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/authentication/socket-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Security
- Software Supply Chain Security
- Dependency Scanning
- Software Composition Analysis
- Vulnerability Management
- Open Source Security
- DevSecOps
- SBOM
- Package Analysis
---
