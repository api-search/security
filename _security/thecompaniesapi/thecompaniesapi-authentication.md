---
api_key_in:
- header
api_specs:
- filename: thecompaniesapi-actions-api-openapi.yml
  format: yaml
  label: The Companies API actions API
  slug: thecompaniesapi-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-actions-api-openapi.yml
- filename: thecompaniesapi-analytics-api-openapi.yml
  format: yaml
  label: The Companies API analytics API
  slug: thecompaniesapi-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-analytics-api-openapi.yml
- filename: thecompaniesapi-companies-api-openapi.yml
  format: yaml
  label: The Companies API companies API
  slug: thecompaniesapi-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-companies-api-openapi.yml
- filename: thecompaniesapi-industries-api-openapi.yml
  format: yaml
  label: The Companies API industries API
  slug: thecompaniesapi-industries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-industries-api-openapi.yml
- filename: thecompaniesapi-job-titles-api-openapi.yml
  format: yaml
  label: The Companies API job-titles API
  slug: thecompaniesapi-job-titles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-job-titles-api-openapi.yml
- filename: thecompaniesapi-lists-api-openapi.yml
  format: yaml
  label: The Companies API lists API
  slug: thecompaniesapi-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-lists-api-openapi.yml
- filename: thecompaniesapi-locations-api-openapi.yml
  format: yaml
  label: The Companies API locations API
  slug: thecompaniesapi-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-locations-api-openapi.yml
- filename: thecompaniesapi-prompts-api-openapi.yml
  format: yaml
  label: The Companies API prompts API
  slug: thecompaniesapi-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-prompts-api-openapi.yml
- filename: thecompaniesapi-teams-api-openapi.yml
  format: yaml
  label: The Companies API teams API
  slug: thecompaniesapi-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-teams-api-openapi.yml
- filename: thecompaniesapi-technologies-api-openapi.yml
  format: yaml
  label: The Companies API technologies API
  slug: thecompaniesapi-technologies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-technologies-api-openapi.yml
- filename: thecompaniesapi-users-api-openapi.yml
  format: yaml
  label: The Companies API users API
  slug: thecompaniesapi-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-users-api-openapi.yml
- filename: thecompaniesapi-utilities-api-openapi.yml
  format: yaml
  label: The Companies API utilities API
  slug: thecompaniesapi-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/openapi/thecompaniesapi-utilities-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Thecompaniesapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Companies API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The Companies API
provider_slug: thecompaniesapi
scheme_count: 1
schemes:
- description: API token passed in the Authorization header, value prefixed "Basic ". Tokens are permanent and managed on the API tokens page in account settings.
  docs: https://www.thecompaniesapi.com/api/authentication
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/thecompaniesapi-actions-api-openapi.yml
  - openapi/thecompaniesapi-analytics-api-openapi.yml
  - openapi/thecompaniesapi-companies-api-openapi.yml
  - openapi/thecompaniesapi-industries-api-openapi.yml
  - openapi/thecompaniesapi-job-titles-api-openapi.yml
  - openapi/thecompaniesapi-lists-api-openapi.yml
  - openapi/thecompaniesapi-locations-api-openapi.yml
  - openapi/thecompaniesapi-prompts-api-openapi.yml
  - openapi/thecompaniesapi-teams-api-openapi.yml
  - openapi/thecompaniesapi-technologies-api-openapi.yml
  - openapi/thecompaniesapi-users-api-openapi.yml
  - openapi/thecompaniesapi-utilities-api-openapi.yml
  - https://www.thecompaniesapi.com/api/authentication
  type: apiKey
  value_format: Basic <api-token>
slug: thecompaniesapi-authentication
source_filename: thecompaniesapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://www.thecompaniesapi.com/api/authentication (docs) + openapi/thecompaniesapi-actions-api-openapi.yml,\n  openapi/thecompaniesapi-analytics-api-openapi.yml, openapi/thecompaniesapi-companies-api-openapi.yml,\n  openapi/thecompaniesapi-industries-api-openapi.yml, openapi/thecompaniesapi-job-titles-api-openapi.yml,\n  openapi/thecompaniesapi-lists-api-openapi.yml, openapi/thecompaniesapi-locations-api-openapi.yml, openapi/thecompaniesapi-prompts-api-openapi.yml,\n  openapi/thecompaniesapi-teams-api-openapi.yml, openapi/thecompaniesapi-technologies-api-openapi.yml,\n  openapi/thecompaniesapi-users-api-openapi.yml, openapi/thecompaniesapi-utilities-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API token passed in the Authorization header, value prefixed \"Basic \". Tokens are permanent\n    and\
  \ managed on the API tokens page in account settings.\n  sources:\n  - openapi/thecompaniesapi-actions-api-openapi.yml\n  - openapi/thecompaniesapi-analytics-api-openapi.yml\n  - openapi/thecompaniesapi-companies-api-openapi.yml\n  - openapi/thecompaniesapi-industries-api-openapi.yml\n  - openapi/thecompaniesapi-job-titles-api-openapi.yml\n  - openapi/thecompaniesapi-lists-api-openapi.yml\n  - openapi/thecompaniesapi-locations-api-openapi.yml\n  - openapi/thecompaniesapi-prompts-api-openapi.yml\n  - openapi/thecompaniesapi-teams-api-openapi.yml\n  - openapi/thecompaniesapi-technologies-api-openapi.yml\n  - openapi/thecompaniesapi-users-api-openapi.yml\n  - openapi/thecompaniesapi-utilities-api-openapi.yml\n  - https://www.thecompaniesapi.com/api/authentication\n  value_format: Basic <api-token>\n  docs: https://www.thecompaniesapi.com/api/authentication\ndocs: https://www.thecompaniesapi.com/api/authentication\nnote: 'The published OpenAPI declares only `apiKey in header: Authorization`\
  \ with no value format. The\n  authentication documentation is explicit that the header value must be prefixed \"Basic \" — `Authorization:\n  Basic MY-API-TOKEN`. A client generated from the spec alone sends a bare token and receives 401 missingApiSecret.\n  Despite the keyword, this is NOT RFC 7617 HTTP Basic: the value is a raw token, not a base64 user:pass\n  pair. Tokens are documented as permanent and never expiring, managed on the API tokens page in account\n  settings. New accounts receive 500 free credits with no credit card.'\ntoken_lifetime: permanent — documented as never expiring\nalternatives:\n- name: token query parameter\n  in: query\n  parameter: token\n  example: https://api.thecompaniesapi.com/v2/companies/{domain}?token=MY-API-TOKEN\n  docs: https://www.thecompaniesapi.com/api/authentication\n  note: Documented as \"mostly used to quickly test an endpoint\". Not declared in the OpenAPI. Places the\n    credential in the URL where it lands in logs, referrers and browser\
  \ history — an agent should use\n    the header.\noauth2: false\nscopes: null\nscopes_note: No OAuth2 and no scope surface; a token carries full account privileges (\"Your API tokens\n  carry many privileges, so keep them secure!\").\nrotation:\n  documented: false\n  note: Tokens can be created and deleted from the settings page; no rotation policy, expiry or key-versioning\n    scheme is published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thecompaniesapi/refs/heads/main/authentication/thecompaniesapi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company Data
- Data Enrichment
- Firmographics
- Web Intelligence
- B2B Data
- Reference Data
- Company Search
---
