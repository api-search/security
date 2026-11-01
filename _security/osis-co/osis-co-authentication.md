---
anonymous_access: false
api_key_in: []
api_specs:
- filename: osis-co-ai-api-openapi.yml
  format: yaml
  label: osis-co AI API
  slug: osis-co-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-ai-api-openapi.yml
- filename: osis-co-calls-api-openapi.yml
  format: yaml
  label: osis-co Calls API
  slug: osis-co-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-calls-api-openapi.yml
- filename: osis-co-capabilities-api-openapi.yml
  format: yaml
  label: osis-co Capabilities API
  slug: osis-co-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-capabilities-api-openapi.yml
- filename: osis-co-conversations-api-openapi.yml
  format: yaml
  label: osis-co Conversations API
  slug: osis-co-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-conversations-api-openapi.yml
- filename: osis-co-events-api-openapi.yml
  format: yaml
  label: osis-co Events API
  slug: osis-co-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-events-api-openapi.yml
- filename: osis-co-groups-api-openapi.yml
  format: yaml
  label: osis-co Groups API
  slug: osis-co-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-groups-api-openapi.yml
- filename: osis-co-lines-api-openapi.yml
  format: yaml
  label: osis-co Lines API
  slug: osis-co-lines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-lines-api-openapi.yml
- filename: osis-co-messages-api-openapi.yml
  format: yaml
  label: osis-co Messages API
  slug: osis-co-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-messages-api-openapi.yml
- filename: osis-co-number-changes-api-openapi.yml
  format: yaml
  label: osis-co Number Changes API
  slug: osis-co-number-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-number-changes-api-openapi.yml
- filename: osis-co-payments-api-openapi.yml
  format: yaml
  label: osis-co Payments API
  slug: osis-co-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-payments-api-openapi.yml
- filename: osis-co-webhooks-api-openapi.yml
  format: yaml
  label: osis-co Webhooks API
  slug: osis-co-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-webhooks-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Osis Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: osis-co declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: osis-co
provider_slug: osis-co
scheme_count: 1
schemes:
- evidence: 'Put your key in the `Authorization` header on every request:'
  header: Authorization
  how_to_obtain: Create a key via the API keys page in the dashboard and copy the generated `COMMS_API_KEY`.
  location: header
  name: Authorization
  type: http-bearer
slug: osis-co-authentication
source_filename: osis-co-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.osis.co/messages-api/authentication.md
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.osis.co/messages-api/authentication.md\nsources:\n- https://docs.osis.co/messages-api/authentication.md\n- https://docs.osis.co/quickstart.md\n- https://docs.osis.co/payments-api/hosted-agents.md\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Put your key in the `Authorization` header on every request:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key via the API keys page in the dashboard and copy the generated `COMMS_API_KEY`.\ndocs: https://docs.osis.co/messages-api/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/osis-co/authentication/osis-co-authentication.yml
summary_line: 1 scheme
tags:
- Messaging
- Communications
- API
- SaaS
- CustomerSupport
---
