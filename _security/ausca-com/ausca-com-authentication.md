---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ausca-com-agent-inboxes-api-openapi.yml
  format: yaml
  label: Ausca Agent Inboxes API
  slug: ausca-com-agent-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-agent-inboxes-api-openapi.yml
- filename: ausca-com-analyze-document-api-openapi.yml
  format: yaml
  label: Ausca Analyze Document API
  slug: ausca-com-analyze-document-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-analyze-document-api-openapi.yml
- filename: ausca-com-artifacts-api-openapi.yml
  format: yaml
  label: Ausca Artifacts API
  slug: ausca-com-artifacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-artifacts-api-openapi.yml
- filename: ausca-com-browser-sessions-api-openapi.yml
  format: yaml
  label: Ausca Browser Sessions API
  slug: ausca-com-browser-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-browser-sessions-api-openapi.yml
- filename: ausca-com-extend-inbox-api-openapi.yml
  format: yaml
  label: Ausca Extend Inbox API
  slug: ausca-com-extend-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-extend-inbox-api-openapi.yml
- filename: ausca-com-extract-text-api-openapi.yml
  format: yaml
  label: Ausca Extract Text API
  slug: ausca-com-extract-text-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-extract-text-api-openapi.yml
- filename: ausca-com-invocations-api-openapi.yml
  format: yaml
  label: Ausca Invocations API
  slug: ausca-com-invocations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-invocations-api-openapi.yml
- filename: ausca-com-lease-browser-api-openapi.yml
  format: yaml
  label: Ausca Lease Browser API
  slug: ausca-com-lease-browser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-lease-browser-api-openapi.yml
- filename: ausca-com-offers-api-openapi.yml
  format: yaml
  label: Ausca Offers API
  slug: ausca-com-offers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-offers-api-openapi.yml
- filename: ausca-com-open-inbox-api-openapi.yml
  format: yaml
  label: Ausca Open Inbox API
  slug: ausca-com-open-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-open-inbox-api-openapi.yml
- filename: ausca-com-transcribe-media-api-openapi.yml
  format: yaml
  label: Ausca Transcribe Media API
  slug: ausca-com-transcribe-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-transcribe-media-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Ausca Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ausca secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ausca
provider_slug: ausca-com
scheme_count: 1
schemes:
- bearerFormat: opaque
  description: Opaque expiry-bound authority for one Ausca resource lease. Never place it in JSON, query parameters, MCP tool arguments, logs, or receipts.
  name: LeaseCapability
  scheme: bearer
  sources:
  - openapi/ausca-com-openapi.json
  type: http
slug: ausca-com-authentication
source_filename: ausca-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/ausca-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: LeaseCapability\n  type: http\n  scheme: bearer\n  bearerFormat: opaque\n  description: Opaque expiry-bound authority for one Ausca resource lease. Never place it in\n    JSON, query parameters, MCP tool arguments, logs, or receipts.\n  sources:\n  - openapi/ausca-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/ausca-com/authentication/ausca-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Pay-per-call APIs
- Agent Infrastructure
- Document OCR
- Media transcription
- Inbox verification
---
