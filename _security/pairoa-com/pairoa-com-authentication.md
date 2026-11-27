---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: pairoa-com-auth-api-openapi.yml
  format: yaml
  label: Pairoa Auth API
  slug: pairoa-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pairoa-com/openapi/pairoa-com-auth-api-openapi.yml
- filename: pairoa-com-contact-api-openapi.yml
  format: yaml
  label: Pairoa Contact API
  slug: pairoa-com-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pairoa-com/openapi/pairoa-com-contact-api-openapi.yml
- filename: pairoa-com-matches-api-openapi.yml
  format: yaml
  label: Pairoa Matches API
  slug: pairoa-com-matches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pairoa-com/openapi/pairoa-com-matches-api-openapi.yml
- filename: pairoa-com-needs-api-openapi.yml
  format: yaml
  label: Pairoa Needs API
  slug: pairoa-com-needs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pairoa-com/openapi/pairoa-com-needs-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Pairoa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pairoa secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Pairoa
provider_slug: pairoa-com
scheme_count: 2
schemes:
- in: header
  name: AnonymousToken
  parameter: X-Anonymous-Token
  sources:
  - openapi/pairoa-com-openapi.yml
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/pairoa-com-openapi.yml
  type: http
slug: pairoa-com-authentication
source_filename: pairoa-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/pairoa-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: AnonymousToken\n  type: apiKey\n  in: header\n  parameter: X-Anonymous-Token\n  sources:\n  - openapi/pairoa-com-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/pairoa-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/pairoa-com/authentication/pairoa-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Matching
- Artificial Intelligence
- Private
- MCP
---
