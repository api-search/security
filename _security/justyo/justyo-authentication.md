---
api_key_in:
- query
- form
api_specs:
- filename: justyo-yo-openapi.yml
  format: yaml
  label: Yo API
  slug: yo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justyo/refs/heads/main/openapi/justyo-yo-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Justyo Authentication
name_suffix: Authentication
oauth_flows: []
overview: justyo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: justyo
provider_slug: justyo
scheme_count: 1
schemes:
- also_in: form
  description: Yo API token issued per registered API username via the Yo Developer Hub.
  in: query
  name: apiToken
  parameter: api_token
  sources:
  - openapi/justyo-yo-openapi.yml
  type: apiKey
slug: justyo-authentication
source_filename: justyo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.justyo.co/ (docs.justyo.co, dev.justyo.co) + openapi/justyo-yo-openapi.yml\ndocs: https://docs.justyo.co/docs/oauth\nsummary:\n  types: [apiKey]\n  api_key_in: [query, form]\n  oauth2_flows: []\n  notes: >-\n    Primary auth is a static Yo API token (api_token) issued per registered API\n    username at the Yo Developer Hub (dev.justyo.co / dashboard.justyo.co). The token\n    is sent as the api_token form field on POST requests and as the api_token query\n    parameter on GET requests. Yo also documented an OAuth 2.0 page (docs.justyo.co/docs/oauth)\n    for delegated \"send on behalf of a user\" access, but the ReadMe hub recorded\n    oauth.enabled=false and the feature was beta; concrete authorize/token URLs are\n    not published, so no oauth2 scheme is asserted here to avoid fabrication.\nschemes:\n  - name: apiToken\n    type: apiKey\n    in: query\n    parameter: api_token\n    also_in: form\n    description:\
  \ Yo API token issued per registered API username via the Yo Developer Hub.\n    sources: [openapi/justyo-yo-openapi.yml]\noauth2_documented:\n  documented: true\n  status: beta-disabled\n  docs: https://docs.justyo.co/docs/oauth\n  note: OAuth 2.0 delegated access was documented but not enabled in the live hub.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/justyo/refs/heads/main/authentication/justyo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Notifications
- Push Notifications
- Messaging
- Mobile
- Developer Tools
- API
---
