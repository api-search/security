---
anonymous_access: false
api_key_in: []
api_specs:
- filename: capmus-com-public-api-openapi.yml
  format: yaml
  label: Capmus Public API
  slug: capmus-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capmus-com/openapi/capmus-com-public-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: none
name: Capmus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Capmus declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Capmus
provider_slug: capmus-com
scheme_count: 0
schemes: []
slug: capmus-com-authentication
source_filename: capmus-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: 'name: Capmus authentication

  generated: ''2026-11-03''

  method: none

  source: https://capmus.com/llms.txt

  docs: https://capmus.com/llms.txt

  schemes: []

  note: The OpenAPI (https://capmus.com/api/public/openapi.json, v1.2.0) declares no securitySchemes and no security requirement, and llms.txt documents all four /api/public endpoints as open to agents without credentials. Write endpoints are gated by human email confirmation instead of API keys (sendMessageToListing emails a confirmation link to reply_to_email; createPostDraft returns a continue_url the poster must open). An unauthenticated GET /api/public/listings?limit=1 returned 200 on 2026-11-03.

  '
source_yaml_url: https://artifacts.apis.io/capmus-com/authentication/capmus-com-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Marketplace
- Classifieds
- Students
- Universities
- Housing
- Job
- Education
---
