---
anonymous_access: false
api_key_in:
- cookie
- header
api_specs:
- filename: openglass-glass-agents-api-openapi.yml
  format: yaml
  label: OpenGlass Agents API
  slug: openglass-glass-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openglass-glass/openapi/openglass-glass-agents-api-openapi.yml
- filename: openglass-glass-attestations-api-openapi.yml
  format: yaml
  label: OpenGlass Attestations API
  slug: openglass-glass-attestations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openglass-glass/openapi/openglass-glass-attestations-api-openapi.yml
- filename: openglass-glass-auth-api-openapi.yml
  format: yaml
  label: OpenGlass Auth API
  slug: openglass-glass-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openglass-glass/openapi/openglass-glass-auth-api-openapi.yml
- filename: openglass-glass-claims-api-openapi.yml
  format: yaml
  label: OpenGlass Claims API
  slug: openglass-glass-claims-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openglass-glass/openapi/openglass-glass-claims-api-openapi.yml
- filename: openglass-glass-invites-api-openapi.yml
  format: yaml
  label: OpenGlass Invites API
  slug: openglass-glass-invites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openglass-glass/openapi/openglass-glass-invites-api-openapi.yml
- filename: openglass-glass-meta-api-openapi.yml
  format: yaml
  label: OpenGlass Meta API
  slug: openglass-glass-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openglass-glass/openapi/openglass-glass-meta-api-openapi.yml
- filename: openglass-glass-owner-api-openapi.yml
  format: yaml
  label: OpenGlass Owner API
  slug: openglass-glass-owner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openglass-glass/openapi/openglass-glass-owner-api-openapi.yml
- filename: openglass-glass-records-api-openapi.yml
  format: yaml
  label: OpenGlass Records API
  slug: openglass-glass-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openglass-glass/openapi/openglass-glass-records-api-openapi.yml
- filename: openglass-glass-sessions-api-openapi.yml
  format: yaml
  label: OpenGlass Sessions API
  slug: openglass-glass-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openglass-glass/openapi/openglass-glass-sessions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: OpenGlass Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenGlass secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OpenGlass
provider_slug: openglass-glass
scheme_count: 2
schemes:
- description: 'Ed25519 signature over sigInput("request", H(JCS({method, path, timestamp, nonce, bodySha256}))).

    Must be sent together with the OG-Agent, OG-Key, OG-Timestamp and OG-Nonce headers (SPEC §4.1).'
  in: header
  name: agentSignature
  parameter: OG-Signature
  sources:
  - openapi/openglass-glass-openapi.yml
  type: apiKey
- in: cookie
  name: ownerSession
  parameter: og_session
  sources:
  - openapi/openglass-glass-openapi.yml
  type: apiKey
slug: openglass-glass-authentication
source_filename: openglass-glass-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/openglass-glass-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: agentSignature\n  type: apiKey\n  in: header\n  parameter: OG-Signature\n  description: |-\n    Ed25519 signature over sigInput(\"request\", H(JCS({method, path, timestamp, nonce, bodySha256}))).\n    Must be sent together with the OG-Agent, OG-Key, OG-Timestamp and OG-Nonce headers (SPEC §4.1).\n  sources:\n  - openapi/openglass-glass-openapi.yml\n- name: ownerSession\n  type: apiKey\n  in: cookie\n  parameter: og_session\n  sources:\n  - openapi/openglass-glass-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/openglass-glass/authentication/openglass-glass-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Artificial Intelligence
- Data Integrity
- Security
- Agent Platform
- Transparency
---
