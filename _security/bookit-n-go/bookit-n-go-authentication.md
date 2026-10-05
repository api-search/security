---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bookit-n-go-agent-api-openapi.yml
  format: yaml
  label: Bookit N Go Agent API
  slug: bookit-n-go-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bookit-n-go/refs/heads/main/openapi/bookit-n-go-agent-api-openapi.yml
- filename: bookit-n-go-flights-api-openapi.yml
  format: yaml
  label: Bookit N Go Flights API
  slug: bookit-n-go-flights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bookit-n-go/refs/heads/main/openapi/bookit-n-go-flights-api-openapi.yml
- filename: bookit-n-go-hotels-api-openapi.yml
  format: yaml
  label: Bookit N Go Hotels API
  slug: bookit-n-go-hotels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bookit-n-go/refs/heads/main/openapi/bookit-n-go-hotels-api-openapi.yml
- filename: bookit-n-go-travelers-api-openapi.yml
  format: yaml
  label: Bookit N Go Travelers API
  slug: bookit-n-go-travelers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bookit-n-go/refs/heads/main/openapi/bookit-n-go-travelers-api-openapi.yml
- filename: bookit-n-go-trips-api-openapi.yml
  format: yaml
  label: Bookit N Go Trips API
  slug: bookit-n-go-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bookit-n-go/refs/heads/main/openapi/bookit-n-go-trips-api-openapi.yml
- filename: bookit-n-go-webhooks-api-openapi.yml
  format: yaml
  label: Bookit N Go Webhooks API
  slug: bookit-n-go-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bookit-n-go/refs/heads/main/openapi/bookit-n-go-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bookit N Go Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bookit N Go secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bookit N Go
provider_slug: bookit-n-go
scheme_count: 1
schemes:
- description: ZOE API sandbox credential (zoe_sandbox_ prefix). X-API-Key is also accepted.
  name: SandboxApiKey
  scheme: bearer
  sources:
  - openapi/bookit-n-go-openapi.yaml
  type: http
slug: bookit-n-go-authentication
source_filename: bookit-n-go-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: derived\nsource: openapi/bookit-n-go-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: SandboxApiKey\n  type: http\n  scheme: bearer\n  description: ZOE API sandbox credential (zoe_sandbox_ prefix). X-API-Key is also accepted.\n  sources:\n  - openapi/bookit-n-go-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bookit-n-go/refs/heads/main/authentication/bookit-n-go-authentication.yml
summary_line: http · 1 scheme
tags:
- Travel
- Software-as-a-Service
- Artificial Intelligence
- White Label
- B2B
---
