---
api_key_in: []
api_specs:
- filename: pact-index-api-openapi.yml
  format: yaml
  label: Pact Index API
  slug: pact-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pact/refs/heads/main/openapi/pact-index-api-openapi.yml
- filename: pact-pacticipants-api-openapi.yml
  format: yaml
  label: Pact Pacticipants API
  slug: pact-pacticipants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pact/refs/heads/main/openapi/pact-pacticipants-api-openapi.yml
- filename: pact-pacts-api-openapi.yml
  format: yaml
  label: Pact Pacts API
  slug: pact-pacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pact/refs/heads/main/openapi/pact-pacts-api-openapi.yml
- filename: pact-verifications-api-openapi.yml
  format: yaml
  label: Pact Verifications API
  slug: pact-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pact/refs/heads/main/openapi/pact-verifications-api-openapi.yml
- filename: pact-webhooks-api-openapi.yml
  format: yaml
  label: Pact Webhooks API
  slug: pact-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pact/refs/heads/main/openapi/pact-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pact Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pact secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pact
provider_slug: pact
scheme_count: 1
schemes:
- description: HTTP Basic authentication (when the broker is configured for it)
  name: basicAuth
  scheme: basic
  sources:
  - openapi/pact-openapi.yml
  type: http
slug: pact-authentication
source_filename: pact-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pact-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication (when the broker is configured for it)\n  sources:\n  - openapi/pact-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pact/refs/heads/main/authentication/pact-authentication.yml
summary_line: http · 1 scheme
tags:
- Contract Testing
- Open-Source
- Testing
---
