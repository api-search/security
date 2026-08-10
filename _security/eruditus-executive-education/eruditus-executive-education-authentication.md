---
api_key_in:
- header
api_specs:
- filename: eruditus-executive-education-leads-api-openapi.yml
  format: yaml
  label: Eruditus Leads API
  slug: eruditus-executive-education-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eruditus-executive-education/refs/heads/main/openapi/eruditus-executive-education-leads-api-openapi.yml
- filename: eruditus-executive-education-programs-api-openapi.yml
  format: yaml
  label: Eruditus Programs API
  slug: eruditus-executive-education-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eruditus-executive-education/refs/heads/main/openapi/eruditus-executive-education-programs-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Eruditus Executive Education Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eruditus secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Eruditus
provider_slug: eruditus-executive-education
scheme_count: 2
schemes:
- description: 'Partner token issued by Emeritus. Per the published reference: "We will provide your own token to use in the requests. Please contact us if you need one."'
  in: header
  name: LeadWebhookKey
  parameter: LEAD_WEBHOOK_KEY
  sources:
  - openapi/eruditus-executive-education-leads-openapi.yml
  type: apiKey
- description: 'Partner token issued by Emeritus. Per the published reference: "We will provide your own token to use in the requests. Please contact us if you need one."'
  in: header
  name: ResourcesApiKey
  parameter: HTTP-EE-RESOURCES-API-KEY
  sources:
  - openapi/eruditus-executive-education-programs-openapi.yml
  type: apiKey
slug: eruditus-executive-education-authentication
source_filename: eruditus-executive-education-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\ndocs: https://emeritus-tech.github.io/emeritus-api-docs/index.html\nsource: openapi/eruditus-executive-education-leads-openapi.yml, openapi/eruditus-executive-education-programs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: LeadWebhookKey\n  type: apiKey\n  in: header\n  parameter: LEAD_WEBHOOK_KEY\n  description: 'Partner token issued by Emeritus. Per the published reference: \"We will provide\n    your own token to use in the requests. Please contact us if you need one.\"'\n  sources:\n  - openapi/eruditus-executive-education-leads-openapi.yml\n- name: ResourcesApiKey\n  type: apiKey\n  in: header\n  parameter: HTTP-EE-RESOURCES-API-KEY\n  description: 'Partner token issued by Emeritus. Per the published reference: \"We will provide\n    your own token to use in the requests. Please contact us if you need one.\"'\n  sources:\n  - openapi/eruditus-executive-education-programs-openapi.yml\n\
  model: static-per-api-token\nissuance:\n  self_service: false\n  process: 'Manual. Published verbatim in the reference: \"We will provide your own token to use\n    in the requests. Please contact us if you need one.\"'\n  contact: https://emeritus.org/connect-with-us/\nnotes:\n- Each API has its own authorization header name — there is no single shared scheme across the\n  Emeritus estate. The reference states this explicitly under \"Authentication\".\n- Tokens are static bearer-equivalents carried in a custom header, not in `Authorization`.\n- No OAuth 2.0, no OpenID Connect, no mTLS, no HTTP basic/bearer. /.well-known/openid-configuration\n  and /.well-known/oauth-authorization-server return 404 on every Emeritus host (probed 2026-08-04).\n- No scope, permission or key-rotation surface is published; scopes/ is therefore not emitted.\n- The same token model applies to both the staging and production environments; no test-vs-live\n  key prefix scheme is published.\nverified:\n  fetched:\
  \ '2026-08-04'\n  evidence:\n  - url: https://admissions.emeritus.org/api/v1/programs_api/programs\n    http_status: 401\n    body: '{\"error\":\"This is not an authorized request\"}'\n  - url: https://admissions.emeritus.org/api/v1/generic_lead\n    method: POST\n    http_status: 401\n    body: '{\"error\":\"This is not an authorized request\"}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eruditus-executive-education/refs/heads/main/authentication/eruditus-executive-education-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Education
- Online Learning
- Executive Education
- EdTech
- Higher Education
- Leads
- Enrollment
- Programs
- Singapore
---
