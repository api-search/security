---
api_key_in:
- header
api_specs:
- filename: retraced-openapi-original.json
  format: json
  label: Retraced Public API
  slug: retraced-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retraced/refs/heads/main/openapi/retraced-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Retraced Authentication
name_suffix: Authentication
oauth_flows: []
overview: Retraced secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Retraced
provider_slug: retraced
scheme_count: 1
schemes:
- description: Set the request header `companyapikey` to the value of an API key created in the Retraced Platform under Developers HQ > API Keys. Keys are shown once at creation. A single key is scoped to both the staging and production environments. If Developers HQ is not visible in the sidebar, a Customer Success Manager must enable it for the account.
  in: header
  name: companyApiKey
  parameter: companyapikey
  sources:
  - openapi/retraced-openapi-original.json
  type: apiKey
slug: retraced-authentication
source_filename: retraced-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://publicapi.retraced.com/\ndocs: https://publicapi.retraced.com/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nnote: >-\n  The Retraced Public API OpenAPI does not declare securitySchemes; the auth model\n  below is captured verbatim from the published API reference. Authentication is\n  passwordless via a company-scoped API key sent in an HTTP header.\nschemes:\n  - name: companyApiKey\n    type: apiKey\n    in: header\n    parameter: companyapikey\n    description: >-\n      Set the request header `companyapikey` to the value of an API key created in the\n      Retraced Platform under Developers HQ > API Keys. Keys are shown once at creation.\n      A single key is scoped to both the staging and production environments. If\n      Developers HQ is not visible in the sidebar, a Customer Success Manager must\n      enable it for the account.\n    sources: [openapi/retraced-openapi-original.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/retraced/refs/heads/main/authentication/retraced-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Applicative Saas
- Supply Chain
- Sustainability
- Compliance
- Fashion
- Traceability
- Digital Product Passport
- ESG
---
