---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: dumpthis-sh-agent-api-openapi.yml
  format: yaml
  label: V Tracer Agent API
  slug: dumpthis-sh-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpthis-sh/openapi/dumpthis-sh-agent-api-openapi.yml
- filename: dumpthis-sh-lifecycle-api-openapi.yml
  format: yaml
  label: V Tracer Lifecycle API
  slug: dumpthis-sh-lifecycle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpthis-sh/openapi/dumpthis-sh-lifecycle-api-openapi.yml
- filename: dumpthis-sh-mcp-api-openapi.yml
  format: yaml
  label: V Tracer MCP API
  slug: dumpthis-sh-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpthis-sh/openapi/dumpthis-sh-mcp-api-openapi.yml
- filename: dumpthis-sh-meta-api-openapi.yml
  format: yaml
  label: V Tracer Meta API
  slug: dumpthis-sh-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpthis-sh/openapi/dumpthis-sh-meta-api-openapi.yml
- filename: dumpthis-sh-relay-api-openapi.yml
  format: yaml
  label: V Tracer Relay API
  slug: dumpthis-sh-relay-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpthis-sh/openapi/dumpthis-sh-relay-api-openapi.yml
- filename: dumpthis-sh-synack-api-openapi.yml
  format: yaml
  label: V Tracer SYNACK API
  slug: dumpthis-sh-synack-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpthis-sh/openapi/dumpthis-sh-synack-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Dumpthis Sh Authentication
name_suffix: Authentication
oauth_flows: []
overview: V Tracer secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: V Tracer
provider_slug: dumpthis-sh
scheme_count: 3
schemes:
- description: Public consent token from /llms.txt. Proves the caller read the docs. Not a secret — not authentication. Endpoints accepting this token also accept anonymous requests.
  in: header
  name: discoveryToken
  parameter: X-SYNACK-DISCOVERY-TOKEN
  sources:
  - openapi/dumpthis-sh-openapi.json
  type: apiKey
- description: Management token from handshake. Self-service lifecycle.
  name: managementToken
  scheme: bearer
  sources:
  - openapi/dumpthis-sh-openapi.json
  type: http
- description: RFC 9421 HTTP Message Signature (Ed25519). Used for node-to-node federation writes. See top-level x-rfc9421 for required headers and replay protection.
  name: federationSignature
  scheme: signature
  sources:
  - openapi/dumpthis-sh-openapi.json
  type: http
slug: dumpthis-sh-authentication
source_filename: dumpthis-sh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/dumpthis-sh-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: discoveryToken\n  type: apiKey\n  in: header\n  parameter: X-SYNACK-DISCOVERY-TOKEN\n  description: Public consent token from /llms.txt. Proves the caller read the docs. Not a secret\n    — not authentication. Endpoints accepting this token also accept anonymous requests.\n  sources:\n  - openapi/dumpthis-sh-openapi.json\n- name: managementToken\n  type: http\n  scheme: bearer\n  description: Management token from handshake. Self-service lifecycle.\n  sources:\n  - openapi/dumpthis-sh-openapi.json\n- name: federationSignature\n  type: http\n  scheme: signature\n  description: RFC 9421 HTTP Message Signature (Ed25519). Used for node-to-node federation writes.\n    See top-level x-rfc9421 for required headers and replay protection.\n  sources:\n  - openapi/dumpthis-sh-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/dumpthis-sh/authentication/dumpthis-sh-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Art
- Artificial Intelligence
- Platform
- Open Source
- Experimental
---
