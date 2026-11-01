---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: J2 Innovations Authentication
name_suffix: Authentication
oauth_flows: []
overview: J2 Innovations declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: J2 Innovations
provider_slug: j2-innovations
scheme_count: 3
schemes:
- description: Salted Challenge Response Authentication Mechanism (RFC5802, RFC7804)
  flow: '1. Hello Handshake: Client sends hello message with username

    2. Server responds with supported authentication mechanisms

    3. Authentication Exchange: Client picks mechanism and exchanges messages

    4. Server sends auth token if authentication successful

    5. Client uses auth token (bearer token) for future requests

    '
  name: SCRAM
  notes: Uses HTTP Authentication framework (RFC7235) with SCRAM mechanism
  type: http
- description: Plaintext authentication (less secure, for testing)
  flow: Similar to SCRAM but with plaintext credentials
  name: PLAINTEXT
  notes: Defined in Haystack specification but less secure than SCRAM
  type: http
- description: Auth token obtained after successful authentication
  format: bearer {token}
  in: header
  name: Bearer Token
  notes: Used for authenticated requests after successful SCRAM or PLAINTEXT authentication
  param_name: Authorization
  type: apiKey
slug: j2-innovations-authentication
source_filename: j2-innovations-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: searched\nsource: https://project-haystack.org/doc/docHaystack/Auth\ndocs: https://project-haystack.org/doc/docHaystack/Auth\nschemes:\n  - name: SCRAM\n    type: http\n    description: Salted Challenge Response Authentication Mechanism (RFC5802, RFC7804)\n    flow: |\n      1. Hello Handshake: Client sends hello message with username\n      2. Server responds with supported authentication mechanisms\n      3. Authentication Exchange: Client picks mechanism and exchanges messages\n      4. Server sends auth token if authentication successful\n      5. Client uses auth token (bearer token) for future requests\n    notes: Uses HTTP Authentication framework (RFC7235) with SCRAM mechanism\n  - name: PLAINTEXT\n    type: http\n    description: Plaintext authentication (less secure, for testing)\n    flow: Similar to SCRAM but with plaintext credentials\n    notes: Defined in Haystack specification but less secure than SCRAM\n  - name: Bearer Token\n\
  \    type: apiKey\n    description: Auth token obtained after successful authentication\n    in: header\n    param_name: Authorization\n    format: bearer {token}\n    notes: Used for authenticated requests after successful SCRAM or PLAINTEXT authentication"
source_yaml_url: https://artifacts.apis.io/j2-innovations/authentication/j2-innovations-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Smart Buildings
- Building Automation
- IoT
- Project Haystack
- Smart Equipment
- Siemens
---
